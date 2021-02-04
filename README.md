## Welcome to SouljaCoin

At the end of January, 2021 [Soulja Boy (Drako)](https://twitter.com/souljaboy) tweeted to "make SouljaCoin a real thing without getting into any legal trouble with SEC etc".

![SouljaBoy SouljaCoin tweet](https://i.imgur.com/zIGi4q9.png)
[https://twitter.com/souljaboy/status/1355178088275959813?s=20](https://twitter.com/souljaboy/status/1355178088275959813?s=20)

So, to make it happen, here is a community built cryptocurrency coin made for Soulja Boy fans. Following are the details:

- Built using Komodo's Antara Smartchain technology
- Independent blockchain
- Block time aprox 60 seconds.
- Block halving every 388885 blocks.
   - aprox every 270.0590278 days
   - aprox every 8.872575862 months
- Block reward of 1 satoshi will reach in about 25.89607116 years.
- Total supply of around 200 million. Exactly to be 199,209,119.99420500 by year 2046+
- 60% blocks are mined with Proof of Work (Equihash)
- 40% blocks are mined with Proof of Stake
- Premine supply of 100,000
- Founders Reward is 1%, mined every 10080 blocks, which is approx of 7 days

## Features

- Coming from Komodo Platform, it is capable of doing all DeFi things one can possible do using Antara Smartchain's Crypto-Conditions technology.
- **Tokens Exchange**, which can be used to create and trade NFTs. [Link](https://developers.komodoplatform.com/basic-docs/antara/antara-api/assets.html)
- **Dilithium** type transactions can make Quantum Resistant transactions [Link](https://developers.komodoplatform.com/basic-docs/antara/antara-api/dilithium.html)
- **Decentralised Faucet**, to give away free SOULJA coins to people who wants to try things out on this chain. [Link](https://developers.komodoplatform.com/basic-docs/antara/antara-api/faucet.html)
- **Heir**, can help manage funds in a way that it can be passed on to heir for inheridence. [Link](https://developers.komodoplatform.com/basic-docs/antara/antara-api/heir.html)
- **Oracles**, to link real world data to blockchain based decentralised applications. Oracles are what powers DeFi. It is very powerful technology. And it works already available to Antara Smartchains. [Link](https://developers.komodoplatform.com/basic-docs/antara/antara-api/oracles.html)
- **Pegs**, to make decentralised stablecoins or making pegged cryptocurrencies to other kind of assets in financial world. [Link](https://developers.komodoplatform.com/basic-docs/antara/antara-api/pegs.html)


## Resources

#### Help/Support Guides
For best staking results, use this guide for staking. Just make sure to use SOULJA instead of example coin name in the guide:
- [https://github.com/kmdlabs/pos64staker](https://github.com/kmdlabs/pos64staker)

#### SouljaCoin Halving detaiils
The detailed halving estimation sheet can be accessed from here:
[https://docs.google.com/spreadsheets/d/1ItLK8xtTjzSyYRgonMKvT1RZQ4lsl1ebnRIFcydVVsQ](https://docs.google.com/spreadsheets/d/1ItLK8xtTjzSyYRgonMKvT1RZQ4lsl1ebnRIFcydVVsQ)

#### Explorer
- [http://explorer.souljacoin.cash/](http://explorer.souljacoin.cash/)
- [http://soulja.explorer.dexstats.info/](http://soulja.explorer.dexstats.info/)

#### Wallets
- [AtomicDEX-Desktop](https://github.com/KomodoPlatform/atomicDEX-Desktop/releases)
- [Command Line](#Using-Command-Line)

#### Connect with SouljaCoin community
- [#soulja channel on Komodo Discord](https://discord.gg/JcNqhUxAxh)

#### Mining Pools
- [https://mining.spaceworks.co](https://mining.spaceworks.co)
- [http://mining.daemoncoins.com/](http://mining.daemoncoins.com/)

#### Exchanges
- [AtomicDEX-Desktop](https://github.com/KomodoPlatform/atomicDEX-Desktop/releases)

#### Using command line
Download pre-compiled komodo binaries for your operating system from [here](https://github.com/KomodoPlatform/komodo/releases/tag/0.6.1).
Extract the binaries, and execute "fetch-params" script from command line terminal to fetch the required chain params.

#### Launch SOULJA Blockchain
Use the following command to connect to SOULJA chain's network:

```bash
./komodod -ac_name=SOULJA -ac_supply=100000 -ac_reward=25600000000 -ac_perc=100000000 -ac_founders=10080 -ac_halving=388885 -ac_pubkey=02fec5cebe47bd5f8eb2ac6f3dff76a82a1292c761d4ccfda578da89f74360c5ee -ac_staked=40 -addnode=51.222.150.53 -daemon
```

#### Mine SOULJA blockchain
Use "-gen" and "-genproclimit" to enable mining. Value for "-genproclimit" is the value of how many CPU threads you have on your system.

```bash
./komodod -ac_name=SOULJA -ac_supply=100000 -ac_reward=25600000000 -ac_perc=100000000 -ac_founders=10080 -ac_halving=388885 -ac_pubkey=02fec5cebe47bd5f8eb2ac6f3dff76a82a1292c761d4ccfda578da89f74360c5ee -ac_staked=40 -addnode=51.222.150.53 -daemon -gen -genproclimit=4
```

#### Wallet comands

```bash
# Get wallet and blockchain info
./komodo-cli -ac_name=SOULJA getinfo


# Get wallet information
./komodo-cli -ac_name=SOULJA getwalletinfo


# Get mining information
./komodo-cli -ac_name=SOULJA getmininginfo


# Generate a new Public address
./komodo-cli -ac_name=SOULJA getnewaddress


# To backup the private key of a public address
./komodo-cli -ac_name=SOULJA dumpprivkey


# To import private key of public address
./komodo-cli -ac_name=SOULJA importprivkey "PRIVATE_KEY_STRING_FROM_DUMPPRIVKEY_COMMAND"


# Generate a new Z/Private address
./komodo-cli -ac_name=SOULJA z_getnewaddress


# To backup the private key of a z address
./komodo-cli -ac_name=SOULJA z_exportkey "zaddr"


# To mine with CPU and enable staking
./komodo-cli -ac_name=SOULJA setgenerate true 0

# To only stake and not CPU mining
./komodo-cli -ac_name=SOULJA setgenerate false 0

# To disable staking and disable CPU mining
./komodo-cli -ac_name=SOULJA setgenerate false 1


# To send mined coins to a z address
./komodo-cli -ac_name=SOULJA "fromaddress" "tozaddress" ( fee ) ( limit )

# Example 1:
./komodo-cli -ac_name=SOULJA z_shieldcoinbase "FROM_YOUR_ADDRESS" "TO_Z_ADDRESS"

# Example 2:
./komodo-cli -ac_name=SOULJA z_shieldcoinbase "*" "TO_Z_ADDRESS"


# To send a transaction from your z address to another z address
./komodo-cli -ac_name=SOULJA z_sendmany "fromaddress" [{"address":... ,"amount":...},...] ( minconf ) ( fee )

# Example:
komodo-cli -ac_name=SOULJA z_sendmany "FROM_Z_ADDRESS" '[{"address": "TO_Z_ADDRESS" ,"amount": 5.9999}]'
```
