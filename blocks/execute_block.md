# Execute Block

This document describes the **Execute Block** user interface component, which provides an interface for executing custom transactions. With this block, the user can execute custom transactions by filling in all the required fields. You can use this block multiple times and anywhere in your task, but it MUST be after the **Start** and **Wallet** blocks.

<img width="960" alt="execute_block" src="https://github.com/user-attachments/assets/3abd21e5-4d56-4861-9560-6f98a40b4d50" />

## 📋 Example

For instance, we examined an ETH deposit transaction within the Moonwell decentralized application on the Base network.
Link on TX - https://basescan.org/tx/0x0c86641194161e7f4888b65f243f8a183ab14a8f5cef6020ce1a1dd4a6586df2

<img width="1689" alt="execute_block" src="https://github.com/user-attachments/assets/5e30ad2a-2a70-454b-87d0-0f24b527a152" />

The `Amount` field is used to specify the required amount of the native network token for the transaction. In the `Gas Price` field, you can set the priority gas price for the transaction. This is an optional parameter; if you don't specify it, the transaction will proceed with the current gas price on the blockchain.

In the `Contract` field, you need to enter the address of the contract to which you are sending the transaction. The `Description TX` field allows you to provide a name for your transaction. It is recommended to use logical names, such as "Moonwell:", since this field serves as a variable that helps you group several **Execute Blocks**. This grouping facilitates the proper mixing of blocks in your task.

The `Input Data` field is the most crucial part of this block, as it contains the data needed to execute the transaction itself. This includes the transaction method (e.g., keccak256) and its parameters in HEX format. In this case, the address of the wallet of the transaction sender is passed as a parameter. However, Kozel includes constant variables, such as <addr> (which represents the wallet address selected in the Wallet Block) and <deadline> (indicating the time to execute the transaction in Timestamp format). You can also create your own variables in the [**Variable Block**](https://github.com/dry-com/kozel/blob/main/blocks/variable_block.md).

## 🖼 Description of block fields

| Field                             | Description                                                                                                        |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------|
| **Amount**                        | The amount of native tokens required to execute a transaction. This field also connects to optional blocks and other data sources, such as **Random Block** or data from other blocks.                    |
| **Gas Price (optional)**          | Priority gas for the transaction is an optional parameter; if you do not specify it, the transaction will proceed at the current gas price on the blockchain.                                    |
| **Contract**                      | The contract to which you are sending the transaction.                                          |
| **Transaction Description**       | The name for your transaction.                |
| **Input Data**                    | Data to execute the transaction, including the transaction method (keccak256) and the parameters of this method (in HEX format).                                      |
| **Clear Button**                  | Resets all fields and removes any connections you’ve made.                                                         |
| **Save Button**                   | Saves and applies the configured execute parameters to the workflow.                                              |


If you have any questions or suggestions, please use the links below:

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HiddenCodeDevs/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/hidden_coding)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@flaming_chameleon)
