# Swap Block

This document describes the **Swap Block** UI component, which provides an interface for performing a swap. With this block, users can perform swaps on the available DEXs based on their selected network in the **Switch Network Block**. Additionally, there is an option for a custom swap, where users need to input the router contract and/or the factory contract, depending on the pool version.

<img width="521" alt="swap_block" src="https://github.com/user-attachments/assets/6580b0d2-ae5f-4a31-9322-670a9a022b7f" />

## 📋 Overview

The block has two types:

- **Default swap**: This is a normal swap that will be done on one of your chosen Dex (if there are Dexs on the network you chose).
- **Custom swap**: This is a custom swap where you need to input the router contract and/or the factory contract, depending on the pool version. It is usually used if your chosen network does not have a supported Dex, or if you want to use a custom swap yourself.

## 🖼 Description of block items

Detailed description of each item in the wallets block:

| Form field                      | Description                                                                                                                                          |
|---------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Enable Custom Swap** Toggle   | Enabling Custom Swap Usage.                                  |
| **Router Contract**             | Enter the router contract.                                                    |
| **Swap Factory Contract**       | Enter the factory contract.       |
| **Add min amount**              | When activating this parameter, you must enter the minimum amount of token that must be in the wallet to make a transfer (if the selected wallet for the transfer has less token than you specified in the Min Amount field, then your task will skip this block for the selected wallet)..                                    |
| **Amount**                      | The amount of tokens you want to send. Also in this field there is a connection point for optional and other blocks. For example **Random Block** or data from other blocks.                      |
| **From Token**                  | Enter the token from which you will make the swap. Also in this field there is a connection point for optional and other blocks. For example **Random Block** or data from other blocks.                      |
| **To Token**                    | Enter the token you want to receive after the swap is completed. Also in this field there is a connection point for optional and other blocks. For example **Random Block** or data from other blocks.                      |
| **Clear Button**                | Clear all block configurations.                                                                                   |
| **Save Button**                 | Saves the current block configuration and applies it to the system.                                                                                  | 

If you have any questions or suggestions, please use the links below:

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HiddenCodeDevs/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/hidden_coding)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@flaming_chameleon)
