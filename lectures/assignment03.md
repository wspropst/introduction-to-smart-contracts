## Instructions
1. Write a getCount() function for the CountContract.sol. This function should simply return the variable count.
2. To test our function we will write a test also using the Solidity language. You will need to set the count to your desired number similar to the testSetCount() function. Also check if the function returns the correct value using assertEq. Reference the testSetCount() and remember to use getCount() instead of count().
3. Compile your contract using npm run compile. Debug as necessary.
4. Test your contract's functions with npm run test.
5. Now you must deploy your contract onto the Goerli chain.
	- First you must fill in your Metamask Private Key. Click on the three dots in the top right, then click account details. You will then need to enter your password to view your private key. Copy and paste this key into each variable ending with PRIVATE_KEY. 
	- Next you must go to alchemy which you signed up for when getting test ETH from the faucet. https://www.alchemy.com/. Create an API key and paste it into the ALCHEMY_API_KEY line within the ENV file.
	- Finally you must make a https://etherscan.io/ account. Then generate an API key using this account. Paste this into the ETHERSCAN_API_KEY.
- Now you can deploy and verify your contract all from the command line. To do this use the following commands:
	1. npx hardhat --network goerli deploy --contract <contract_name>
	2. npx hardhat --network goerli verify <deployed_contract_address>
		- You might have to wait a couple minute before you can verify the contract. Make sure to use the address you receive from the first command for the address to verify in the second command.
- Search for you address on the goerli etherscan and try reading and writing the functions in your contract by connecting with MetaMask.
- Either submit your contract address or the goerli etherscan url of the contract address. 