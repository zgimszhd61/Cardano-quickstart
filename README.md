要快速开始使用Cardano链，你需要遵循一系列步骤来设置开发环境、构建和运行Cardano节点，以及创建和使用智能合约。以下是一个基于提供的信息的简化指南：

## 设置开发环境

首先，你需要设置Linux环境，因为Cardano节点和CLI（命令行界面）主要支持Linux平台。Ubuntu 20.04是推荐的操作系统版本。你可以选择在物理机上直接安装Ubuntu，使用虚拟机（VM），或者通过Windows的WSL2运行Ubuntu[1]。

## 安装Cardano节点和CLI

1. **安装依赖**：Cardano节点的构建需要安装一些依赖，包括libsodium库。你可以通过克隆libsodium的GitHub仓库，然后编译和安装它来满足这个依赖[1]。

2. **克隆和构建Cardano节点**：接下来，克隆Cardano节点的GitHub仓库，检出最新的标签版本，并构建它。这将生成两个二进制可执行文件：`cardano-node`和`cardano-cli`[1]。

## 配置节点

配置节点涉及设置节点配置文件、创世文件和拓扑文件。这些配置文件告诉节点如何与Cardano网络的不同时代（如Mary、Alonzo、Babbage等）进行交互[2]。

## 运行和监控节点

运行节点后，你可以通过`cardano-cli`与节点交云，查询网络状态和内部指标。这对于开发DApps、钱包、集成工具、铸造自定义代币或运营自己的权益池至关重要[1]。

## 创建和使用智能合约

1. **设置Plutus开发环境**：Plutus是Cardano上用于智能合约开发的语言。你需要安装GHC和Cabal，以及一些C库，如libblst、libsecp256k1和libsodium。如果你不使用Nix，你需要手动安装这些依赖[6]。

2. **创建新的Cabal包**：创建一个新的目录并初始化一个Cabal包。这个包将构建一个可执行文件，用于你的智能合约[6]。

3. **编写智能合约**：使用Plutus Tx编写智能合约的链上验证器。Plutus Tx支持GHC v9.2.x和v9.6.x版本。你可以参考Plutus文档来学习如何编写和编译智能合约[6]。

4. **与智能合约交互**：一旦你有了验证器，你可以使用高级的离链库和框架，如`cardano-wallet-js`、`cardano-serialization-lib`或`purescript-cardano`，来部署和与智能合约进行交互。这些框架提供了生成密钥对、查询UTXO、构建和提交交易等功能[6]。

通过遵循这些步骤，你可以快速开始在Cardano链上开发。记住，这只是一个快速入门指南，详细的信息和指导请参考提供的资源。

Citations:
[1] https://learn.lovelace.academy/getting-started/running-a-full-node/
[2] https://docs.cardano.org/cardano-testnet/getting-started/
[3] https://www.youtube.com/watch?v=hzMH2LnzZ90
[4] https://docs.cardano.org/native-tokens/getting-started/
[5] https://docs.cardano.org/cardano-sidechains/sidechain-toolkit/introduction/
[6] https://plutus.readthedocs.io/en/latest/quick-start.html
[7] https://www.reddit.com/r/cardano/comments/lnj5ne/getting_started_guide_a_newbies_guide_to_cardano/
[8] https://www.youtube.com/playlist?list=PL3CmFT-BByVdWPdCZOIIMVEN2R5qxMQV4
