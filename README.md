# KardiaChain Token Assets
This repository contains information about all the verified token on Aris Mainnet of KardiaChain Network.
All the unverified tokens will be marked as "unverified token". The verified tokens' logo and information will be displayed on the Token page, Search box, Transfers section and other places on the KardiaChain Network Explorer so users can easily determinate the trusted projects.

## Prerequisites
1. The token contract source code **must be verified** on the KardiaChain Explorer.
2. Folk this Github repository.
3. Create a folder inside **token** folder with the name of Token Contract Address as checksum format
`token/<token_address_checksum>`
Example: `token/0xAF984E23EAA3E7967F3C5E007fbe397D8566D23d`
4. Upload the token logo inside the folder and name it **logo.png**
The image must be in **PNG** format, transparent background, size 128x128px and filesize is less than 50kb with good resolution.
Example: `token/0xAF984E23EAA3E7967F3C5E007fbe397D8566D23d/logo.png`
5. Create a **data.json** file inside the folder
Example: `token/0xAF984E23EAA3E7967F3C5E007fbe397D8566D23d/data.json`
The data file contains information about the project, for example:
```
{
	"contract": "0xAF984E23EAA3E7967F3C5E007fbe397D8566D23d",
	"type": "KRC-20",
	"name": "WKAI",
	"symbol": "WKAI",
	"decimals": 18,
	"description": "Wrapped KAI (WKAI) is a token that represents KAI 1:1 and conforms to the KRC20 token format. WKAI KRC20 increases the token's functionality, including but not limited to dApps on KardiaChain ecosystem. DApps might require users to convert KAI to WKAI and you can unwrap your WKAI to KAI 1:1 at any time.",
	"website": "https://kaidex.io/wkai",
	"github": "",
	"telegram": "",
	"medium": "",
	"twitter": "",
	"facebook": ""
}
```

	+ *(Required)* contract: the token contract address in checksum format
	+ *(Required)* type: token format (KRC-20, KRC-721, KRC-1155)
	+ *(Required)* name: name of token must match the deployed token's name
	+ *(Required)* symbol: token symbol must match the deployed token's symbol
	+ *(Required)* decimals: token symbol must match the deployed token's decimals
	+ *(Required)* description: short introduction about the project
	+ *(Required)* website: main website of the project
	+ *(Required)* github: source code of the project
	+ *(Optional)* telegram, medium, twitter, facebook: social links

7. Create a pull request to the **master** repository and wait for the verification process.
8. The fee for the verification is **500 KAI** (dynamic, change over time)
After your pull request meets the requirements, send the payment to the following address on KardiaChain Aris Mainnet **0xE8A5B3C80551E48c5a527a473FbbaCceF858Bbdb** and provide the transaction hash.

## Policy
1. We do not verify the functions that develop on the token contract (eg: mint() function of the token's owner, pause() transfer or trading forbidden...)
2. We do not verify other source codes, smart contracts that implementation on top of the token contract.
3. We do not guarantee the business model of the projects or behaviors of the token's owner.
5. Unverified token does not mean the token is not legit, token's owner can still verify the source code of the token contract without adding logo.
4. Do your own research and invest at your own risk.

## Where is the token logo and infomation located?
+ Default logo of unverified token <img src="https://raw.githubusercontent.com/kardiachain/token-assets/master/tokens/default.png" width="24">

+ Verified token logo will be displayed on the explorer including token page, search bar, token transfer section and so on
<img src="https://raw.githubusercontent.com/kardiachain/token-assets/master/samples/sample_1.png" width="250">
<img src="https://raw.githubusercontent.com/kardiachain/token-assets/master/samples/sample_2.png" width="250">