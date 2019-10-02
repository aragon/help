 The EURS token contract has a fee mechanism that might not be playing nicely with how the Aragon frontend calculates token approvals.

The Finance app's Finance.deposit() does a transferFrom() under the hood. The EURS token, on transferFrom(), transfers:

1. The requested amount from the holder to the finance app
2. A set "fee" amount from the holder to the "fee collector"

Both the requested amount and the set fee amount require approvals from the holder for the Finance app (since Finance is the contract making the transferFrom() call), but right now the Finance app only requests approval for the first transfer. So when a user attempts to deposit EURS using the Finance app, the fee amount hasn't been approved and the second transfer for the fee fails, reverting the entire transaction.

It should be noted this "fee" mechanism implemented by EURS is not a part of the ERC20 standard. The EURS token claims to be "ERC20-compliant", but adjusting the transferFrom() like it has for this mechanism makes EURS incompatible with the ERC20 standard. Under the ERC20 standard there is a 1:1 approval to transfer ratio, but the extra fee transfer implemented by EURS changes this assumption and will likely break a lot of existing token-handling contracts.

There is no way to work around this right now using just the Aragon frontend client because the Finance contract also assumes a 1:1 approval to transfer ratio. Users can send EURS directly to their organization's Vault app address and then make a withdrawal using the aragonCLI.
