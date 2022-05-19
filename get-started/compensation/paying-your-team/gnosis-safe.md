---
description: How to use the csv airdrop to pay your team
---

# Gnosis Safe

* Log into your safe
* Click apps, search Csv, and select CSV Airdrop
  1. ![](<../../../.gitbook/assets/image (12).png>)
*   Format your Coordinape csv correctly:

    Preparing a Transfer File

    Transfer files are expected to be in CSV format with the following required columns:

    * **`token_type`**: The type of token that is being transferred. One of `erc20,nft` or `native`. NFT Tokens can be either ERC721 or ERC1155.
    * **`token_address`**: Ethereum address of ERC20 token to be transferred. This has to be left blank for native (ETH) transfers.
    * **`receiver`**: Ethereum address of transfer receiver.
    * **`amount`**: the amount of token to be transferred. This can be left blank for erc721 transfers.
    * **`id`**: The id of the collectible token (erc721 or erc1155) to transfer. This can be left blank for native and erc20 transfers.

    **Important: The CSV file has to use "," as a separator and the header row always has to be provided as the first row and include the described column names.**
* Upload your csv and click submit.&#x20;
  1. ![](<../../../.gitbook/assets/image (30).png>)
