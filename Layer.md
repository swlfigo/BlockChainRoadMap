# 什么是Layer1、Layer2

![layer](http://sylarimage.oss-cn-shenzhen.aliyuncs.com/uPic/qs9OyE.png)



## What is layer 1?

Layer 1网络是底层[区块链](https://academy.binance.com/zh/articles/what-is-blockchain-technology-a-comprehensive-guide-for-beginners)的别称。[币安智能链](https://academy.binance.com/zh/articles/an-introduction-to-binance-smart-chain-bsc)(BNB)、[以太坊](https://academy.binance.com/zh/articles/what-is-ethereum)(ETH)、[比特币](https://academy.binance.com/en)(BTC)和[Solana](https://academy.binance.com/zh/articles/what-is-solana-sol)都属于Layer-1协议。我们称之为Layer 1，是因为它们是所在生态系统中的主要网络。与之相对的链下解决方案和Layer 2解决方案都是在主链上搭建的。

换言之，Layer 1协议能够在自身的区块链上处理并完成交易，同时自带用于支付交易费用的原生[代币](https://academy.binance.com/en/glossary/token)。



Layer 1 is the base blockchain. Ethereum and Bitcoin are both layer 1 blockchains because they are the **underlying foundation that various layer 2 networks build on top of**. Examples of layer 2 projects include "rollups" on Ethereum and the Lightning Network on top of Bitcoin. All user transaction activity on these layer 2 projects can ultimately settle back to the layer 1 blockchain.

Ethereum also functions as a data availability layer for layer 2s. Layer 2 projects will post their transaction data onto Ethereum, relying on Ethereum for data availability. This data can be used to get the state of the layer 2, or to dispute transactions on layer 2.

**Ethereum as the layer 1 includes:**

1. **A network of node operators** to secure and validate the network
2. **A network of block producers**
3. **The blockchain** itself and the history of transaction data
4. **The consensus mechanism** for the network



Layer2 的链以Layer1为基础开发



# The challenge of decentralized scaling

Layer1 遇到的难点，任何公链都在找三者的平衡点。

为了解决拥堵,交易费贵问题.提出2个解决方案: 

* Layer2
* 升级Layer1



![J5rmkw](https://sylarimage.oss-cn-shenzhen.aliyuncs.com/uPic/J5rmkw.png)



# What is layer 2?

Layer 2 (L2) is a collective term to describe a specific set of Ethereum scaling solutions. **A layer 2 is separate blockchain that extends Ethereum and inherits the security guarantees of Ethereum**.

Layer2 与 Layer1 完全分开，不是同一条链。在Layer1上扩展，继承Layer1的安全性。

Layer2 解决 Layer1 问题方案: 2种 RollUps 技术



# Why do we need layer 2?

Three desirable properties of a blockchain are that it is **decentralized, secure, and scalable**. The [blockchain trilemma](https://www.ledger.com/academy/what-is-the-blockchain-trilemma) states that a simple blockchain architecture can only achieve two out of three. Want a secure and decentralized blockchain? You need to sacrifice scalability.

Ethereum has reached the network's current capacity with [1+ million transactions per day](https://etherscan.io/chart/tx) and high demand for each of these transactions. The success of Ethereum and the demand to use it has caused gas prices to rise substantially. Therefore the need for scaling solutions has increased in demand as well. This is where layer 2 networks come in.

### Scalability

The main goal of scalability is to increase transaction speed (faster finality) and transaction throughput (higher transactions per second) without sacrificing decentralization or security.

The Ethereum community has taken a strong stance that it would not throw out decentralization or security in order to scale. Until [sharding](https://ethereum.org/en/upgrades/sharding/), Ethereum Mainnet (layer 1) is only able to process [roughly 15 transactions per second](https://ethtps.info/Network/Ethereum). When demand to use Ethereum is high, the network becomes congested, which increases transaction fees and prices out users who cannot afford those fees. That is where layer 2 comes in to scale Ethereum today.

[More on Ethereum's vision](https://ethereum.org/zh/upgrades/vision/)

当前主网15笔交易/秒。造成拥堵



# Rollups

Rollups are currently the preferred layer 2 solution for scaling Ethereum. By using rollups, users can [reduce gas fees by up to 100x](https://l2fees.info/) compared to layer 1.

Rollups bundle (or ’roll up’) hundreds of transactions into a single transaction on layer 1. This distributes the L1 transaction fees across everyone in the rollup, making it cheaper for each user. **Rollup transactions get executed outside of layer 1 but the transaction data gets posted to layer 1**. By posting transaction data onto layer 1, rollups inherit the security of Ethereum. There are two different approaches to rollups: optimistic and zero-knowledge - they differ primarily on how this transaction data is posted to L1.

Rollups技术减少100x gas fee,把公链上几百个交易打包成1个交易。没笔交易平摊gas交易费。打包操作在Layer 1外，但最终处理完会打包回Layer1上，有点Redis缓存意思。



# The need for upgrades

Layer1 升级

## The Merge

- Soon, the current Ethereum Mainnet will merge with the Beacon Chain proof-of-stake system.
- This will mark the end of proof-of-work for Ethereum, and the full transition to proof-of-stake.
- This sets the stage for future scaling upgrades including sharding.
- The Merge will reduce Ethereum's energy consumption by ~99.95%.

POW -> POS



## Reference

[什么是区块链中的Layer 1？ | Binance Academy](https://academy.binance.com/zh/articles/what-is-layer-1-in-blockchain)

[Layer 2 | ethereum.org](https://ethereum.org/zh/layer-2/#main-content)

[Ethereum vision | ethereum.org](https://ethereum.org/en/upgrades/vision/#main-content)