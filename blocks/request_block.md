# Request Block

This document describes the **Request Block** user interface component, which provides an interface for receiving and then saving data from the blockchain. With this block, users can request various types of data, including the number of tokens in a wallet, the amount of tokens available for minting, and any other data that has a read function. The received data is stored in a variable named according to the recommendation provided in the `Description TX` field, which corresponds to the name used in the [**Execute Block**](https://github.com/dry-com/kozel/blob/main/blocks/execute_block.md#:~:text=The%20Description%20TX%20field%20allows%20you%20to%20provide%20a%20name%20for%20your%20transaction.%20It%20is%20recommended%20to%20use%20logical%20names%2C%20such%20as%20%22Moonwell%3A%22%2C%20since%20this%20field%20serves%20as%20a%20variable%20that%20helps%20you%20group%20several%20Execute%20Blocks.%20This%20grouping%20facilitates%20the%20proper%20mixing%20of%20blocks%20in%20your%20task.). This variable can then be utilized in other blocks, such as the **Execute Block**.

<img width="1004" alt="request_block" src="https://github.com/user-attachments/assets/26ca1da1-db3c-43a0-8faf-886612b99c5c" />

## 📋 Example

In this example, the **Request Block** is utilized to receive and store (in the <Swap: Amount_token> variable) the amount of random tokens after a swap. The variable <Swap: Amount_token> can be utilized in other blocks, such as the Execute Block.

<img width="1289" alt="request_block_example" src="https://github.com/user-attachments/assets/fa64fda2-444c-4889-80ee-d88e7e246ec0" />

In the `Contract` field, we utilize a random token contract from the **Random Block**, which will receive the request. 

The `Description TX` field lets you assign a name to your request and future variable. It is advisable to use logical and descriptive names to help group multiple **Execute Block**. This grouping makes it easier to integrate the blocks effectively within your task.

The `Input Data` field is the most important part of this block, as it contains the data needed to execute the request. This includes the transaction method (e.g. keccak256) and its parameters in HEX format. In this case, the address of the wallet of the transaction sender is passed as a parameter. However, Kozel includes constant variables, such as <addr> (which represents the wallet address selected in the Wallet Block) and <deadline> (indicating the time to execute the transaction in Timestamp format). You can also create your own variables in the [**Variable Block**](https://github.com/dry-com/kozel/blob/main/blocks/variable_block.md).

## 🖼 Description of block fields

| Field                                    | Description                                                                                         |
|------------------------------------------|-----------------------------------------------------------------------------------------------------|
| **Contract**                             | Text field labeled “Contract” – enter the target contract address. This field also connects to optional blocks and other data sources, such as **Random Block** or data from other blocks.                                   |
| **Transaction Description**              | Text field for the query name and future variable.      |
| **Input Data**                           | Data to execute the request, including the transaction method (keccak256) and the parameters of this method (in HEX format).                            |
| **Clear Button**                         | Clears all inputs and resets connections.                                                           |
| **Save Button**                          | Saves and applies the configured request settings.                                                 |



If you have any questions or suggestions, please use the links below:

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HiddenCodeDevs/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/hidden_coding)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@flaming_chameleon)
