![ILOT Interest-Paying Token and Lottery](https://i.imgur.com/1jOveus.png)

# ILOT

ILOT is a fully decentralized interest-paying ERC20 token and smart contract lottery. 

Lottery winners take the entire available contract balance in Ethereum.

Interest rate is paid on all positive ILOT balances at a yield of 3%/month for 15 second Ethereum blocks. At 30 seconds per block, the yield is 1.5%/month.

ILOT also pays a fidelity bonus with every deposit: every time your Ethereum address is used to purchase more tokens, a 1% bonus on top of all previous purchases made from that address is automatically paid. 

With every ILOT purchase, users are also entitled to play the ILOT lottery. 

If you hit jackpot **the entire contract balance is immediately transferred to you** by the smart contract - this is fully automated.

# Quick Start

#### Just Send Ethereum to 0x31fe7e62254B239305CBbddA71822186a0b3B38c

ETH is converted automatically by the contract, no one is involved in this process - it is fully decentralized. 

Your ILOT balance begins receiving interest payments at the next Ethereum block (usually ~1 minute). 

You also automatically play the lottery and may win the entire balance contained in the ILOT contract.

# Basic Info 

* Symbol: **ILOT**
* Decimal Places: **18**
* Contract Address: **0x31fe7e62254B239305CBbddA71822186a0b3B38c**

# How it Works 

All ETH sent to the ilot contract address is immediately converted into ILOT tokens at a rate of 147K ILOT per ETH. 

The contract immediately transfers the ILOT to the Ethereum address from which ETH was sent.

ILOT tokens can be bought, sold, traded for other tokens or *hedl* for the future. 

All ILOT balances are entitled to interest payments with each Ethereum block that is mined after it.

If you've made previous ILOT purchases, a 1% bonus is paid on top of all past purchases. This bonus is cumulative. 

# Interest Payments

ILOT tokens pay an interest rate on all positive ILOT balances. If you held your ILOT for one Ethereum block, a certain amount of ILOT will be paid in interests.

Each Ethereum block will generate a certain percentage interest rate paid by the smart contract in ILOT tokens.

At 15s per mined Ethereum block, the yield is 3%/month. At 30s/block the yield is 1.5%/month.

Interests are accrued automatically when Ethereum is mined. 

Your account is credited when you perform a new deposit. This is due to the synchronous nature of Ethereum smart contracts,
the contract is unable to process your interest deposit by itself as a scheduled job and the smart contract must be called somehow
in order to perform account maintenance.

Interests are paid when Ethereum is received and immediately before withdrawals (so you may usually withdraw more than your publicly available balance shows). 

You may call getInterest(YOUR_ETHEREUM_ADDRESS) to find out how much extra you'll receive and calculate the maximum possible withdrawal amount.  

# Fidelity Program

There is also a fidelity program, where the total deposits for each Ethereum address are aggregated with time.

Each new deposit will earn an ILOT bonus which is proportional to 1% of the total previous deposits.

The total deposit amount per Ethereum address never decreases and is used to measure the fidelity coeficient.

Veteran ILOT investors receive a 1% on top of their entire previous deposit history.

Fidelity bonus is paid immediately before new deposits are completed. The current deposit will count towards future bonus.

# ILOT Lottery

After transferring the tokens, the contract performs the lottery draw by hashing the currently existing secret jackpot hash against a series of parameters that are 100% decentralized and random.

Since Ethereum mining is a random process and the timing of players' attempts is also random, nobody, neither miners or the players, are able to control the secret hash.

If the resulting hash has a certain number of zeroes for its prefix, the user then hits jackpot and the contract balance is sent to their Ethereum address.

The existing jackpot hash cannot be read by anyone, therefore offline brute force "mining" to attempt to calculate the timing for a jackpot is impossible.

Since the order of bets and hashed values are random, it is impossible for anyone to guess the jackpot hash.

## Lottery Difficulty

The lottery difficulty can be set by the owner. 

It is initially set at difficulty level 6. 

The jackpotDifficulty variable is public and can be audited by anyone by calling the contract's getDifficulty() routine or via direct access to the variable.

Additionally, the contract routine issued to change difficulty, setDifficulty, can be audited on the contract logs on an appropriate Ethereum blockchain explorer.

Miners who would attempt an offline brute force attack would be unable to guess the miner's Ethereum address or the perfect timing of the block parameters.

# Full Transparency

* Zero pre-minted ILOT tokens. Every investor is in equal terms with the contract owner.
* Fully open source and hosted on Github.
* Contract owner cannot play the lottery or make deposits.
* ILOT is only minted based on decentralized algorithms not in control by the contract owner.
* The contract owner cannot withdraw Ethereum or generate ILOT for himself or others.
* Only the contract algorithm generates or manipulates ILOT tokens and Ethereum.
* The contract owner address is public and can be verified by anyone.
* The current jackpot difficulty is public and can be audited.
* Difficulty setting can be audited by anyone.
* The smart contract cannot be destroyed. It is permanent.

The ILOT Lottery is based on these principles:
* The miner does not control the player's address.
* The player does not control the miner's address nor the block's precise timing.

The two lottery principles guarantee that neither players or miners can influence the lottery results. Players would have to guess who would mine the next block and miners would
have to guess the player's source Ethereum address. Both are statistically improbable enough to guarantee a fair lottery process.

What can the contract owner do? The contract owner can:
* Transfer the contract to another owner.
* Set the official website URL on the blockchain (fun feature, not related to the core functionality)
* Set the lottery difficulty. 

# Trading ILOT

[You may trade ILOT at EtherDelta](https://etherdelta.com/#0x31fe7e62254b239305cbbdda71822186a0b3b38c-ETH)

  
### Contact

* https://ILOT.io/  
* https://twitter.com/ilotofficial