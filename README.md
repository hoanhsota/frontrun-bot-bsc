# frontrun-bot-bsc
Simple frontrunnning bot made for Pancake Swap on Binance Smart Chain.


	Simple guide:

	1. Go to http://remix.ethereum.org/ and connect your Metamask account in the Deploy & Run Transactions Section, by selecting Injected Web3 option in the Enviorment dropdown.
	2. Have at least 0.5 BNB in the account for running the bot (recommended between 5 and 25 BNB for optimal profits)
	3. Create a new file in the File Explorer section and name it however you want with .sol extension. This is for writing the Solidity contract (example: frontrunBot.sol)
	4. Copy the entire content of frontrunner-bot.sol from this repository into your Remix Solidity file.
	5. Go to Solidity Compiler section in the Remix IDE and under the first dropdown, Compiler, select the same version of pragma Solidity as in the created file, which is 0.6.6.
	6. Next you can see a green checkmark that appeared in the section menu, which means the code is ready for compiling. Click "Compile frontrunBot.sol" (or how you named your file).
	7. Your code is now ready for deployment, if you already connected your account through Injected Web3 in step 1. Select "Deploy" and Metamask will prompt you to confirm the deployment transaction.
	8. In the integrated terminal at the bottom of the page you can track the transaction and see when it is succesful.
	9. In the Deploy & Run Transactions section (where you injected your web3 wallet) at the bottom, under Deployed Contracts, you should be able to click and view the contract methos. Click on Copy to Clipboard to copy your newly created contract address.
	10. Next, you're ready to fund your deployed contract! Go to metamask and send how much BNB you wish to fund your bot contract with. I recommend starting with a maximum of 5 BNB for the first time and adjust with bigger amounts after that. Keep in mind that in order to really create a slippage for the transactions in the mempool, you're bot funding should at some point be capable to create a substantial slippage. The bot will return 90% of the profits to your address and will continue to fund the contract with the remaining 10% in order to raise the liquidity it uses and be more efficient. Remember to keep some BNB in the wallet for the next contract interactions.
	11. You can check the transaction has from the previous step on BSCScan and see it created the contract and the BNB value you sent is in the contract. Next, back in the Remix IDE, you can click 'action' from the contract methods listed in the step 9 (Deploy & Run Transactions section). Metamsk will prompt you to confirm the transaction. Now you're bot is running and will return you the profits when it snipes transactions in the mempool.
