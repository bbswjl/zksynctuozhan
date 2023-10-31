zkSync CLI 工具
此 CLI 工具简化了开发应用程序和与 zkSync 2.0 交互的过程。

要求
节点/NPM
纱
用法
您可以使用全局安装此程序npm i -g zksync-cli或使用 npx 直接运行命令npx zksync-cli@latest {COMMAND}。

命令
zksync-cli create {PROJECT_NAME}: 在给定的项目名称中创建一个新的 Hardhat 项目。如果未提供，则在当前文件夹中创建项目，尽管这要求文件夹为空。

zksync-cli deposit：从L1（Goerli testnet）存入资金到zkSync 2.0 testnet。它将要求输入：收款人钱包、ETH 金额（例如 0.1）以及您要从中发送资金的钱包的私钥。

zksync-cli withdraw：从 zkSync 2.0 中提取资金到 L1（Goerli 测试网）。它将要求输入：收款人钱包、ETH 金额（例如 0.1）以及您要从中发送资金的钱包的私钥。

存款和取款都可能需要几分钟才能完成。

开发新功能
安装和构建
安装所有依赖项npm i。这个项目是用 Typescript 构建的。运行npm run build以将代码编译/src成/bin.

要创建版本运行：

git tag v0.1.3    // with the correspondent tag
git push --tags  
测试
适当的测试将很快包括在内。现在，您可以通过使用npm i -g.