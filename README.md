# 2021Wanxiang-Blockchain-Hackathon-AmaraLink

## AmaraLink

The [Amaralink](https://bridge.amara.link/#/) is a cross-chain bridge protocol.This is the code for NodeJs version.

***

## AmaraLink Introduction

- AmaraLink is a data cross-chain bridge of multisignature threshold technology, striving to become an crypto data conversion hub connecting Polkadot and other public chains. 
- At the current stage, we are developing a bridge to connect Moonriver and Polygon/Ethereum. We hope to conduct a demonstration in October to further improve it. 
It will be officially open to all users after the audit.

## Design Overview

**Note：** *Take Solana and Moonriver as examples*

### From SOL(SPL Standard) to MOVR(ERC20 Standard)

![img](https://lh4.googleusercontent.com/ZBKrCrKv6cpQEul5gufkx8CzUO6euzyXedllyIPD0HhN_vkQHGuOX5vQih_rZwOxybGz6P1AeW5jXJxpSSr_Wm-cGfocDkSClcXMUV58ZqDNxAauG27kjaW0QBSlY5b6RTHGbxS6=s1600)

### From MOVR(ERC20 Standard) to SOL(SPL Standard) 

![img](https://lh5.googleusercontent.com/E5VmWL_8q0k1lwIe_AbhaHbZj0WehoeoAsk-UONzt7PgBA2AgsLFzSYJqiAcFMkuarDcwmg3BcrYm7mgnFqSJHiLZ9SFMG_E4b_sTLPAUYiWpYGt2ufzYQV7YOfZdWDjDzLjiNTi=s1600)



## Demo Description

AmaraLink now connects the Moonbase Alpha with the Polygon testnet Mumbai-Testnet, and it will take a few days to apply it to Moonriver Mainnet and Polygon Mainnet.



### **Preparations before testing:**

You will need gas and test coins before testing. For example, if you want your assets cross from Moonbase Alpha to Mumbai-Testnet, test-assets on Moonbase Alpha network and gas DEV are required; conversely, if it’s from Mumbai-Testnet to Moonbase Alpha, then test-assets on Mumbai-Testnet and gas MATIC are required.



### **Moonbase Alpha：**

> RPC [configuration](https://docs.google.com/document/d/1coHhl6UN8sYkKUVEnuyVii0F8W7bPDIUFBfuF6uBOMc/edit#heading=h.eubhpwcb1b7q)
>
> Name: Moonbase-alpha
>
> RPC URL: https://rpc.testnet.moonbeam.network
>
> Chain ID: 1287
>
> Symbol: DEV



Doc. ref：https://docs.moonbeam.network/builders/get-started/moonbase/#get-tokens/

**Here to get gas fee**: DEV https://discord.com/invite/PfpUATX



![img](https://lh4.googleusercontent.com/Rigrztidvqb5c8LzEvDYQKq08PSSb9VizHGsj8Nu2z4kZEaUY1m76v-38W9eStEgUlAWn10ICiLRZrK34dHUkwlaytjw9I5-cQi6_KIFjJTe72hP4I9jucNxL4Qvd_Z47UUkvPQJ=s1600)



Instruction format to check account balance:!balance <enter-address-here->-Instruction format to get DEV:!faucet send <enter-address-here-

**Note：**   *you can only send 1 request every 24 hours for 5DEV*

**Test assets: BTC、USDT、DOT、KSM** 

| Test asset | Contract address                           |
| ---------- | ------------------------------------------ |
| BTC        | 0xD50E4638B5f58A66a5F4FF81F092Db2357EcC6FB |
| KSM        | 0xF4693eD43c9c691c4bAEc0648223B2A6Aaf26583 |
| DOT        | 0x167aCF3d633b9693B9cB4BCcE060f9178D4bAA8D |
| USDT       | 0x0b77D7BDd78b2a4C2c50980968166D99e321DfB6 |
|            |                                            |

Here to get test assets:https://discord.com/invite/rhkyBmmCBfGo to Amara Finance Discord-Faucent-testnet-amara channel- send instruction!drip 0x地址 (note：!drip+space+addr.)



### Mumbai-Testnet (Polygon testnet)：

> Name：Mumbai/Polygon testnet
>
> **RPC URL：**
>
> > https://rpc-mumbai.maticvigil.com
> >
> > https://matic-mumbai.chainstacklabs.com
> >
> > https://matic-testnet-archive-rpc.bwarelabs.com
>
> Chain ID：80001
>
> Symbol：MATIC



Doc. ref: https://docs.polygon.technology/docs/develop/network-details/network

Gas fee：MATICHere to get: [https://faucet.matic.network](https://faucet.matic.network/)

![img](https://lh3.googleusercontent.com/x0nO2ly0hpFAjWfMTRm_-1Ng4E6c5cNc1M2ddurU5CZCs4fMbdg1zVQZF7PrY0yTBXeLWlD7DH_RPIZjirTTnuFS1fONGKAU5aoIwI6mYcY1gQ13qxHzU_eeikcdzTrg3qULifCx=s1600)
**Doc. ref：**

> https://rpc-mumbai.matic.today  
>
> https://matic-mumbai.chainstacklabs.com 
>
> https://rpc-mumbai.maticvigil.com 
>
> https://matic-testnet-archive-rpc.bwarelabs.com



**Test assets ：USDT、FIL、BTC、KSM、DOT**

| Test Assets | Contract address                           |
| ----------- | ------------------------------------------ |
| USDT        | 0x58aE10d450eabC0E9cD03C878Ba4c6b0768d7569 |
| BTC         | 0x7353F1812588033a6dB3687144dC8938252f23f3 |
| KSM         | 0xf1f0741ddD2D78bc7D71A836d75997f0eB2B0d2d |
| DOT         | 0x20C34f982Affae7e33E8140888C7fa82061d4A1C |

*Mumbai test-assets can not be claimed by faucet bot in discord for now.*

```
address: "0x58aE10d450eabC0E9cD03C878Ba4c6b0768d7569", decimals: 18, symbol: "USDT"address: "0x88ded5A6d9D591762C0FD1118eDBeb2F0cF71b4C", decimals: 8, symbol: "FIL" address: "0x7353F1812588033a6dB3687144dC8938252f23f3", decimals: 8, symbol: "BTC" address: "0xf1f0741ddD2D78bc7D71A836d75997f0eB2B0d2d", decimals: 8, symbol: "KSM" address: "0x20C34f982Affae7e33E8140888C7fa82061d4A1C", decimals: 8, symbol: "DOT"
```



### **About cross-chain fee：**

The cross-chain fee of AmaraLink:Take USDT as an example, if the asset needs to cross from Moonbase Alpha to Polygon testnet, users will pay gas(DEV) and handling fee (USDT), which is set to be one . Vice versa.



### **About transaction inquiry:**

- Moonbase Alpha block explorer：https://moonbase-blockscout.testnet.moonbeam.network/
- Polygon testnet block explorer：https://mumbai.polygonscan.com/



## Useful Links
- AmaraLink website：https://bridge.amara.link/#/
- AmaraLink Video（Chinese）：https://youtu.be/zFLzv-X7UBs
- AmaraLink video（English)：https://youtu.be/-j0Pzd7LN6w

## Follow us
- Webiste：https://www.amara.link/
- Discord：https://discord.com/invite/rhkyBmmCBf
- Telegram：https://t.me/AmaraFinance
- Twitter：https://twitter.com/AmaraFinance
- Medium：https://amara-finance.medium.com
