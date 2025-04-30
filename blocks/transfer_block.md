# Transfer Block

This document describes the **Transfer Block** UI component that allows users to make token transfers. The transfer is made from the wallet that was selected in the **Wallets Block** and comes to the recipient's wallet from the input field. You can also implement token transfers to multiple wallets in the block by switching the slider to `To many wallets` and selecting. You can use this block multiple times and anywhere in your task, but it **MUST** be after the Start and Wallet blocks.

<img width="520" alt="Снимок экрана 2025-04-30 в 18 40 46" src="https://github.com/user-attachments/assets/98b96d37-1a82-4a7e-9b5a-9fe774a513ba" />

## 📋 Overview

The block has two types:

- **Single Transfer**: This type of block makes a transfer to one wallet from the input field.
- **Multiple Transfer**: This type of block makes a transfer to the selected wallets from the list. (uses the list of your connected wallets in Kozel).

## 🖼 Component Layout and Controls

| Form field                   | Description                                                                                           |
|------------------------------|-------------------------------------------------------------------------------------------------------|
| **Token**                    | Enter the token contract you want to send.                            |
| **Add min amount**           | When activating this parameter, you must enter the minimum amount of token that must be in the wallet to make a transfer (if the selected wallet for the transfer has less token than you specified in the Min Amount field, then your task will skip this block for the selected wallet)..                                    |
| **Amount**                   | The amount of tokens you want to send.                      |
| **To single wallet**         | Position off, if transfer to one wallet. Position on, if transfer to multiple wallets.                     |
| **Wallet address**           | Recipient wallet address.         |
| **Group Filter Dropdown**    | A dropdown menu labeled "Select group". Select a wallet group to filter the list accordingly.                                                        |
| **Search Wallets**           | A text field with placeholder "Search wallets by Address". Type in an address (e.g., `0x12a5...51bc9`) to filter the wallet list in real time.       |
| **Select All Checkbox**      | A master checkbox that selects or deselects all currently visible wallets in the list.                                                               |
| **Wallet Entry Checkbox**    | Individual checkboxes for each wallet address (e.g., `0x12a5...51bc9`). Use these to block specific wallets one by one.                             |
| **Clear Button**             | Resets type selection and all delay inputs to their defaults.                                         |
| **Save Button**              | Saves the current delay configuration and applies it to the workflow.                                 |

If you have any questions or suggestions, please use the links below:

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HiddenCodeDevs/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/hidden_coding)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@flaming_chameleon)
