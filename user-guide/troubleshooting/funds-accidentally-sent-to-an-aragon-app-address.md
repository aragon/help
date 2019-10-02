<p>
	 If you accidentally send tokens to the address of an app installed in an Aragon organization, you can recover the tokens and send them to the organization's Vault by following these steps:
</p>
<ol>
	<li><a href="https://hack.aragon.org/docs/cli-intro.html" target="_blank">Install the aragonCLI</a> which is a command line interface for interacting with Aragon organizations.</li>
	<li>Run <code>aragon ipfs</code> in your Terminal in order to provide aragonCLI with a way to access data (e.g. ABIs) for Aragon organizations.</li>
	<li><a href="https://hack.aragon.org/docs/guides-faq#set-a-private-key" target="_blank">Set a private key for the aragonCLI to use</a>, then send some ether to the address for this private key to pay for gas.</li>
	<li>Send the following transaction from the aragonCLI, replacing each "address" with the corresponding address relevant to your stuck transaction:</li>
</ol>
<pre>
dao exec OrganizationAddress AppAddress recoverToVault TokenContractAddress --environment aragon:mainnet
</pre>
<p>
	 Where the OrganizationAddress is the address of the organization housing the stuck funds, the AppAddress is the address of the app you sent the stuck funds to, and the TokenContractAddress is the address of the token contract for the token you sent.
</p>
<p>
	 For example, if you sent 
	<a href="https://etherscan.io/token/0x89d24A6b4CcB1B6fAA2625fE562bDD9a23260359" target="_blank">Dai</a> to the Finance app address of the <a href="https://mainnet.aragon.org/#/genesis/settings" target="_blank">genesis.aragonid.eth</a> organization, then the transaction you would send to from the aragonCLI would be:
</p>
<pre>
dao exec 0x8A83D4bCE45b4C4F751f76cf565953D1E4A3BF0a 0x98516C82Bda8B3dE6E2670B718848949Ae6a4643 recoverToVault 0x89d24A6b4CcB1B6fAA2625fE562bDD9a23260359 --environment aragon:mainnet
</pre>
<p>
	 Thanks to Chris Hobcroft for documenting these steps in 
	<a href="https://github.com/ethereum-cat-herders/funding/issues/2#issuecomment-477174751" target="_blank">this GitHub comment</a>.
</p>
