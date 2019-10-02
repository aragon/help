<h4>2.5.1 Navigate to <a href="https://app.aragon.org">https://app.aragon.org</a> in your web browser</h4>
<p>
	 Enable your account, select which network you want to use to create your organization, then click "Create an organization".
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d826d982c7d3a7e9ae152a1/file-sTnfeEGIqe.png">
</p>
<h4 id="select"><a href="#select">2.5.2 Select the “Reputation” template</a></h4>
<p>
	 A “Reputation” organization that uses non-transferable tokens to represent reputation. Decisions are made using reputation-weighted voting, where one reputation token equals one vote.
</p>
<p>
	 Click "View details", review the apps available, check the boxes to install any optional apps you want to install, then click "Use this template".
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d826f0204286364bc8f463b/file-AgyjSpxvPa.png"><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d8270a52c7d3a7e9ae152cc/file-S87GDeFw8Z.png">
</p>
<h4 id="claim"><a href="#claim">2.5.3 Claim a name then click “Next”</a></h4>
<p>
	 Aragon uses the 
	<a href="https://ens.domains/">Ethereum Name Service</a> (ENS) to assign names to organizations.
</p>
<p>
	<em>Note: The organization's ENS name currently cannot be changed.<br>
	</em>
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d82707f04286364bc8f464b/file-BxAkkYMy8r.png">
</p>
<h4 id="set"><a href="#set">2.5.4 Configure the parameters of the Voting app</a></h4>
<p>
	<em>Note: </em><em>The Voting app parameters currently cannot be changed from the Aragon frontend client. To change the Voting app parameters after your organization has been created, you must first initialize the permissions to change these parameters, then you can change the parameters using the <a href="https://hack.aragon.org/docs/cli-intro.html">aragonCLI</a>.</em>
</p>
<p>
	<strong>Support</strong>
</p>
<p>
	 “Support” is the percentage of votes on a proposal that the total "Yes" votes must be greater than for the proposal to be passed. For example, if “Support” is set to 51%, then more than 51% of the votes on a proposal must vote “Yes” for the proposal to pass.
</p>
<p>
	<strong>Minimum Approval %<br>
	</strong>
</p>
<p>
	 "Minimum Approval %" is the percentage of the total token supply that support for a proposal must be greater than for the proposal to be considered valid. For example, if the “Minimum Approval %” is set to 20%, then more than 20% of the outstanding token supply must vote "Yes" on a proposal for the vote to be considered valid.
</p>
<p>
	<strong>Vote Duration</strong>
</p>
<p>
	 “Vote Duration” is the length of time that the vote will be open for participation. For example, if the Vote Duration is set to 24 hours, then tokenholders have 24 hours to participate in the vote. After the 24 hours is over, if the vote does meet the Minimum Approval % and/or Support requirements, then the vote will automatically fail. If the vote meets the Minimum Approval % and Support requirements by the end of the Vote Duration, then the vote will automatically be passed. This parameter cannot be changed after the organization is created.
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d82756404286364bc8f467b/file-4eq8iDevcC.png">
</p>
<h4 id="choose"><a href="#choose">2.5.5 Choose a token name and symbol and add tokenholders</a></h4>
<p>
	<em>Note: The token name and symbol currently cannot be changed. Do not add more than a few tokenholders to your organization on this screen or the transaction to create your organization may fail; you can add more tokenholders after the organization has been created.<br>
	</em>
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d8276df2c7d3a7e9ae1530c/file-XrrkJVkBPW.png">
</p>
<h4 id="review"><a href="#review">2.5.6 Review organization information</a></h4>
<p>
	 Open each panel to make sure that the information entered to launch your organization is correct. If anything is incorrect, you can click the "back" button to return to an earlier screen and make the necessary corrections.
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d82783404286364bc8f469b/file-2gWKfSnRrh.png"><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d82783c04286364bc8f469c/file-IEOzSaKD4d.png"><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d82784304286364bc8f469d/file-5NoBZmLf5p.png"><img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d82784c04286364bc8f469e/file-lVOkTuwMej.png">
</p>
<h4 id="launch"><a href="#launch">2.5.7 Launch your organization</a></h4>
<p>
	 Now you need to sign a transaction to create your organization. Open your Ethereum provider if the window does not open automatically. Click the "confirm" button in your Ethereum provider to sign and broadcast the transaction.
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d8278ca04286364bc8f46a8/file-6TVWa1EJXO.png">
</p>
<h4 id="started"><a href="#started">2.5.8 Click "Get started"</a></h4>
<p>
	 Your new Reputation organization is ready to go!
</p>
<p>
	Now you can 
	<a href="https://help.aragon.org/article/33-explore-the-reputation-organization" target="_blank">explore your new reputation organization</a>.
</p>
<p>
	<img src="https://s3.amazonaws.com/helpscout.net/docs/assets/5c98a4fe0428633d2cf3fcf7/images/5d82792304286364bc8f46b2/file-hFeIf8cLA5.png">
</p>
