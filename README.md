# Poloniex Verify Address

## Background

Poloniex launches [Proof of Reserves (PoR)](https://poloniex.com/topic/security/proof-of-reserves) to improve the security and transparency of user's assets. These tools will allow
you to independently audit Poloniex's Proof of Reserves, verify all Poloniex's reserves addresses known liabilities to
users, in order to confirm the solvency of Poloniex.

## Introduction

### Building the source

Download the [latest build](https://github.com/poloniex/tools-nodejs-address-verify/releases) for your operating system and architecture. Also, you can build the source by yourself.

Building this open source tool requires Node.js (version >= 14.20.0).

Install dependencies
```shell
 npm install 
```

build
```shell
npm run build
```

test
```shell
npm test
```

compile
```shell
npm run compile
```

### Executable

Proof-of-Reserves executable are in the cmd directory

|    Command    | Description                                                                                                                                                                     |
| :-----------: |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   `VerifyAddress`    | We have signed a specific message with a private key to each address published by Poloniex. This tool can be used to verify Poloniex's signature and verify Poloniex's ownership of the address. |

## Reserves

Download Poloniex's [Proof of Reserves File](), verify the ownership of the Poloniex's public address [Details here]()

### VerifyAddress

Poloniex's public file contains address, message "poloniex" and signature. You can use VerifyAddress to verify
Poloniex's ownership of published address.

How to use?

```shell
./VerifyAddress --help
```

![cli-help.png](assets/cli-help.png)

Verify address example:
```shell
./VerifyAddress --por_csv_filename ./poloniex_por_xxxxyyzz.csv
```

The result like below:
![result-summary.png](assets%2Fresult-summary.png)

### VerifyOnline

At the same time, you can use third-party tools to verify the ownership.
- [BTC single addresses](https://www.bitcoin.com/tools/verify-message/)
- [EVM](https://etherscan.io/verifiedsignatures)
- [TRX addresses](https://tronscan.org/#/tools/verify-sign)
