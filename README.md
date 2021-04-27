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
- Founders Reward is ~~1%~~ 100%, mined every 10080 blocks, which is approx of 7 days
- Due to miscalculations 99% Founders Rewards are burned to keep Founders Rewards 1% only. Refer to the [NOTICE](#notice) section to know more.

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

SpaceCoin guide also is relevant to SOULJA staking. Follow it from here:
- [https://github.com/SpaceWorksCo/guides/blob/master/Setup-Staking-Node.md](https://github.com/SpaceWorksCo/guides/blob/master/Setup-Staking-Node.md)

#### SouljaCoin Halving detaiils
The detailed halving estimation sheet can be accessed from here:
[https://docs.google.com/spreadsheets/d/1ItLK8xtTjzSyYRgonMKvT1RZQ4lsl1ebnRIFcydVVsQ](https://docs.google.com/spreadsheets/d/1ItLK8xtTjzSyYRgonMKvT1RZQ4lsl1ebnRIFcydVVsQ)

#### Explorer
- [http://explorer.souljacoin.cash/](http://explorer.souljacoin.cash/)
- [http://soulja.explorer.dexstats.info/](http://soulja.explorer.dexstats.info/)
- [http://soulja.kmdtools.xyz/](https://soulja.kmdtools.xyz/)

#### Wallets
- [AtomicDEX-Desktop](https://github.com/KomodoPlatform/atomicDEX-Desktop/releases)
- [Command Line](#Using-Command-Line)

#### Connect with SouljaCoin community
- [#soulja channel on Komodo Discord](https://discord.gg/JcNqhUxAxh)

#### Mining Pools
- [https://mining.spaceworks.co](https://mining.spaceworks.co)
- [http://mining.daemoncoins.com/](http://mining.daemoncoins.com/)
- [https://unimining.net/](https://unimining.net)
- [http://chickenpool.com/](http://chickenpool.com/)

#### Exchanges
- [AtomicDEX-Desktop](https://github.com/KomodoPlatform/atomicDEX-Desktop/releases)
- [CexZ](https://www.cexz.ca/trading/souljabtc)

#### Using command line
Download pre-compiled komodo binaries for your operating system from [here](https://github.com/KomodoPlatform/komodo/releases/tag/0.6.1).
Extract the binaries, and execute "fetch-params" script from command line terminal to fetch the required chain params.

#### Launch SOULJA Blockchain
Use the following command to connect to SOULJA chain's network:

```bash
./komodod -ac_name=SOULJA -ac_supply=100000 -ac_reward=25600000000 -ac_perc=100000000 -ac_founders=10080 -ac_halving=388885 -ac_pubkey=02fec5cebe47bd5f8eb2ac6f3dff76a82a1292c761d4ccfda578da89f74360c5ee -ac_staked=40 -addnode=49.12.127.114 -addnode=49.12.127.113 -addnode=49.12.127.111 -addnode=51.91.61.195 -addnode=88.99.150.139 -addnode=84.38.189.208 -addnode=46.255.254.134 -addnode=51.83.186.192 -addnode=88.99.212.81 -addnode=159.69.201.122 -addnode=116.203.56.98 -addnode=46.255.254.133 -addnode=94.130.38.173 -addnode=178.63.47.105 -addnode=147.135.105.85 -addnode=95.217.44.58 -addnode=144.76.148.155 -addnode=143.244.47.112 -addnode=141.0.149.92 -addnode=77.244.75.34 -addnode=144.76.148.154 -addnode=152.89.104.58 -addnode=219.138.73.109 -addnode=178.32.41.81 -addnode=103.231.91.233 -addnode=141.0.149.92 -daemon
```

#### Mine SOULJA blockchain
Use "-gen" and "-genproclimit" to enable mining. Value for "-genproclimit" is the value of how many CPU threads you have on your system.

```bash
./komodod -ac_name=SOULJA -ac_supply=100000 -ac_reward=25600000000 -ac_perc=100000000 -ac_founders=10080 -ac_halving=388885 -ac_pubkey=02fec5cebe47bd5f8eb2ac6f3dff76a82a1292c761d4ccfda578da89f74360c5ee -ac_staked=40 -addnode=49.12.127.114 -addnode=49.12.127.113 -addnode=49.12.127.111 -addnode=51.91.61.195 -addnode=88.99.150.139 -addnode=84.38.189.208 -addnode=46.255.254.134 -addnode=51.83.186.192 -addnode=88.99.212.81 -addnode=159.69.201.122 -addnode=116.203.56.98 -addnode=46.255.254.133 -addnode=94.130.38.173 -addnode=178.63.47.105 -addnode=147.135.105.85 -addnode=95.217.44.58 -addnode=144.76.148.155 -addnode=143.244.47.112 -addnode=141.0.149.92 -addnode=77.244.75.34 -addnode=144.76.148.154 -addnode=152.89.104.58 -addnode=219.138.73.109 -addnode=178.32.41.81 -addnode=103.231.91.233 -addnode=141.0.149.92 -daemon -gen -genproclimit=4
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

## Notice

Soon after first Founders Rewards block was mined, it was identified the Founders Rewards calculation was wrong. It was supposed to 1%, but with extra zeros added to the Founders Rewards, it is instead 100%. Means every 10080 blocks, the same amount of the supply equals to the (per block mining reward * 10080) is mined to the Founders Rewards address [RSr5pG3SMVweUxoATEoBrKY9W7KPFAiSZb](https://explorer.souljacoin.cash/address/RSr5pG3SMVweUxoATEoBrKY9W7KPFAiSZb).

As a solution, to keep the Founders Rewards 1%, 99% funds from Founders Rewards are sent to the burn address: [RD6GgnrMpPaTSMn8vai6yiGA7mN4QGPVMY](https://explorer.souljacoin.cash/address/RD6GgnrMpPaTSMn8vai6yiGA7mN4QGPVMY)

Some reference screenshots about this incident as a notification to SOULJA community in discord:

<p align="center">
	<img src="https://raw.githubusercontent.com/satindergrewal/souljacoin.cash/main/images/founders_rewards_calc_screw_up.png" width="500">
</p>

<p align="center">
	<img src="https://raw.githubusercontent.com/satindergrewal/souljacoin.cash/main/images/founders_rewards_99_perc_burned.png" width="100%">
</p>

<p align="center">
	<img src="https://raw.githubusercontent.com/satindergrewal/souljacoin.cash/main/images/warning_about_founders_reward_screw_up.png" width="100%">
</p>
