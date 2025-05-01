# Variable Block

  This document describes the **Variable Block** user interface component, which provides an interface for creating and saving a custom variable for your task.This block enables users to create variables for use in **Execute Blocks**. It is particularly useful for applying randomization within a **Random Block**, especially if the variable's value is uncertain.

  <img width="1101" alt="variable_block" src="https://github.com/user-attachments/assets/29010f4f-fa2c-4091-8773-0c51b96e87d9" />

  ## 📋 Example
  
<img width="1237" alt="variable_block_example" src="https://github.com/user-attachments/assets/23042af4-7dd2-4b23-b5c2-e9425989f451" />

In this example, we utilized a combination of **Random Block** and **Variable Block**. This approach ensures that the <Amount_token> variable is randomized each time we apply our task. And we can apply it in `Input Data` inside the **Execute Block**.

## 🖼 Description of block fields

| Field                                | Description                                                                                               |
|--------------------------------------|-----------------------------------------------------------------------------------------------------------|
| **Variable Symbol**                  | Text field for naming your variable.                                            |
| **Input Data Field**                 | In this field, you need to enter a HEX value that is 64 characters long. This field is also linked to the random block and is automatically converted to 64 HEX characters.       |
| **Clear Button**                     | Resets all inputs and severs any block connections.                                                       |
| **Save Button**                      | Saves the configured variable and makes it available for downstream blocks.                               |
