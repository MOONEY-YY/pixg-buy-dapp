# PIXG 代币一键购买 DApp

[![Base](https://img.shields.io/badge/Chain-Base-blue.svg)](https://basescan.org)
[![Contract](https://img.shields.io/badge/Contract-0xc6f8b19d3a5b85f40a0b3b8e3e73f2d-green.svg)](https://basescan.org/address/0xc6f8b19d3a5b85f40a0b3b8e3e73f2d)

PIXG 是 Base 链上功能 ERC20 代币。用户存 USDT 自动铸造 PIXG 并添加流动性到 Uniswap V2 池子。LP 代币归创建者。

## 代币规格
- **名称**：PIXG
- **符号**：PIXG
- **总量**：1 亿枚 (18 位小数)
- **汇率**：1 USDT = 10,000 PIXG
- **USDT 地址**：0xfde4C96c8593536E31F229EA8f37b2ADa2699bb2 (Base USDT, 6 位小数)
- **合约地址**：0xc6f8b19d3a5b85f40a0b3b8e3e73f2d
- **Uniswap V2 Router**：0x4752ba5DBc23f44D87826276BF6Fd6b1C372aD24

## 功能
- **magicDeposit**：一笔 tx 完成 approve USDT + mint PIXG + 加 LP (价格固定 1:10,000)。
- **限制**：总量 1 亿；1% 滑点保护。

## 一键购买网站
- 访问: https://mooney-y.github.io/pixg-buy-dapp
- 连 MetaMask (Base 链) > 输入 USDT 金额 > 点击 “买 PIXG” > Sign + Confirm tx > 得 PIXG + LP 添加。

## 部署教程
1. Remix: https://remix.ethereum.org > 新文件 `SuperPIXG.sol` > 粘贴代码 > Compile (0.8.20) > Deploy (USDT 参数 0xfde4C96c8593536E31F229EA8f37b2ADa2699bb2) > 验证 Basescan。
2. 代码: [SuperPIXG.sol](SuperPIXG.sol)

## 风险
- 小额测试。
- LP 仅 owner 可撤。

开源欢迎贡献！Twitter: @你的账号
