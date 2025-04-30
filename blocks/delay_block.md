# Delay Block

This document describes the **Delay Block** user interface component, which allows users to insert a custom wait/delay step into their workflow in three ways: statically, randomly, and progressively. You can insert this block anywhere and use it multiple times, but it **MUST** follow the Start and Wallet blocks.

<img width="392" alt="delay_block" src="https://github.com/user-attachments/assets/d9100952-8fd6-401f-89c1-673b39e61267" />

## 📋 Overview

The block has three types:

- **Static Delay**: This block type uses a static delay in seconds. 
- **Progress Delay**: This block type uses a progressive delay in seconds, which consists of a minimum delay, a maximum delay, and a delay between each wallet in seconds.  
- **Random Delay**: This block type uses a random delay in seconds, which consists of a minimum, maximum delay in seconds. 

## 🖼 Component Layout and Controls

| Form field                   | Description                                                                                           |
|------------------------------|-------------------------------------------------------------------------------------------------------|
| **Type Dropdown**            | A select field labeled “Type” with options: `Static`, `Progress`, `Random`.                            |
| **Static Delay Input**       | When `Static` is selected: a text field labeled “Delay” (seconds).                                    |
| **Min Delay Input**          | When `Progress` or `Random` is selected: a field labeled “Min delay” (seconds).                      |
| **Max Delay Input**          | When `Progress` or `Random` is selected: a field labeled “Max delay” (seconds).                      |
| **Delay Between Input**      | When selecting `Progress`: the field labeled "Delay between" (seconds) is the increment of the step between wallets.         |
| **Clear Button**             | Resets type selection and all delay inputs to their defaults.                                         |
| **Save Button**              | Saves the current delay configuration and applies it to the workflow.                                 |

If you have any questions or suggestions, please use the links below:

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HiddenCodeDevs/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/hidden_coding)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@flaming_chameleon)
