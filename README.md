# solana-nft-airdrop
Airdrop a list of Solana token addresses (including NFTs) to a list of wallet addresses. 

## Installation
Clone the latest commit to your machine by clicking 'Code' and then 'Download Zip'.

## Prerequisites
* [Solana Tool Suite](https://docs.solana.com/cli/install-solana-cli-tools)
* [spl-token command line utility](prerequisite)
* [Python 3.9 or higher](https://www.python.org/downloads/release/python-3913/)
* ```TOKEN``` set in solana-airdrop.py
* A list of Solana wallet addresses. These should also be formatted as 1 per line in wallet_list.txt.
* You must use the command: ```solana config set -k <your key file>``` to ensure that the currently selected wallet contains all the tokens listed in token_list.txt.
* The Solana wallet should have enough funds to cover the airdrop and account creation costs.

## Usage
* Open command prompt
* Navigate to the repo directory ```cd /users/tom/github/solana-nft-airdrop```
* Run the python script using command ```python3 solana-nft-airdrop.py```
* Any failed transactions will appear in the command prompt.
* A succesful airdrop will print ```Airdrop #1 Complete``` to the command prompt.
* Once all tokens have been airdropped ```DONE``` will be printed.

## Airdrop costs
* It costs 0.00204428 Solana to airdrop a token to a wallet that does not already have an account corresponding to the sent token.
