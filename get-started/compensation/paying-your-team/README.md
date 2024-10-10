---
description: After the Epoch completes
---

# 💲 Paying Your Team

#### When you are ready to pay your team, these are the options:

* CSV Export&#x20;
* Disperse
* Gnosis Safe
* Parcel&#x20;

![Admin Epoch History](<../../../.gitbook/assets/Export CSV.gif>)

### CSV

With CSV export from your Epoch, you can use this to integrate with your preferred payment method.

Since this is a CSV, you can use this file to pay your team however you'd like and on any chain you'd like; know that the addresses your contributors used to sign in are the ETH mainnet addresses.

### Payment Disbursement

If you're paying your team on Ethereum, you can use any options below, pay them in individual transactions or a custom script.

<details>

<summary>Disperse</summary>

In the [Disperse ](broken-reference/)app after you have your csv you can distribute the tokens you wish to allocate by pasting the token address into the token address section

<img src="../../../.gitbook/assets/image (2) (1) (1) (1).png" alt="" data-size="original">

Then you'll need to take the address and the amount and paste it into the box below.

<img src="../../../.gitbook/assets/image (3) (1) (1) (1).png" alt="" data-size="original">

When you're done, make sure it looks ok and then, click approve and then disperse token

<img src="../../../.gitbook/assets/image (1) (1) (1) (1).png" alt="" data-size="original">

</details>

<details>

<summary>Gnosis Safe</summary>

* Log into your safe

<!---->

* Click apps, search Csv, and select CSV Airdrop
  1. ![](<../../../.gitbook/assets/image (2) (1) (1).png>)

<!---->

*   Format your Coordinape csv correctly:

    Preparing a Transfer File

    Transfer files are expected to be in CSV format with the following required columns:

    * **`token_type`**: The type of token that is being transferred. One of `erc20,nft` or `native`. NFT Tokens can be either ERC721 or ERC1155.
    * **`token_address`**: Ethereum address of ERC20 token to be transferred. This has to be left blank for native (ETH) transfers.
    * **`receiver`**: Ethereum address of transfer receiver.
    * **`amount`**: the amount of token to be transferred. This can be left blank for erc721 transfers.
    * **`id`**: The id of the collectible token (erc721 or erc1155) to transfer. This can be left blank for native and erc20 transfers.

    **Important: The CSV file has to use "," as a separator and the header row always has to be provided as the first row and include the described column names.**

<!---->

* Upload your csv and click submit.
  1. ![](<../../../.gitbook/assets/image (4) (1) (3).png>)

</details>

<details>

<summary>Parcel</summary>

With this integration, Parcel operators can now view the details of each Circle, the status of Epochs with the corresponding list of participants & allocated GIVE scores directly on Parcel. The budget determined by the operator is automatically distributed as per GIVE scores in a simple flow through Parcel saving them from costly errors & hours of admin work.

Coordinape integration can be found under the integrations tab on the navbar from the [Parcel site](https://app.parcel.money)

**Prerequisite :** Wallet address signed into Parcel should be an admin of the Coordinape Circle. If you don’t have a Coordinape Circle already, log in to Coordinape and [create a circle here](https://app.coordinape.com/new-circle).

Steps to follow :

**1. Go to Integrations tab. click on Coordinape**

![](<../../../.gitbook/assets/image (7) (1) (1).png>)

**2. Connect your Coordinape account**\
You will be asked to sign a message that gives us permissions to access your Coordinape data.

**Note:** We do not do any kind of write operations to your Coordinape circles. We use these permissions only to get the details of your circles and epochs.

**3. It will display all the circles on Coordinape associated with the connected wallet**![](<../../../.gitbook/assets/image (11) (1).png>)

Click on any of the circles to view all the epochs of that circle.![](<../../../.gitbook/assets/image (6) (2).png>)

**Note:** You can only create payouts for completed epochs.

**4.  To view all the participants of the circle, click on** <mark style="color:blue;">**View Participants**</mark> **button in the top right corner to view all the participants of the circle.**![](<../../../.gitbook/assets/image (14) (2) (1).png>)

**5. Clicking on** <mark style="color:blue;">**Pay**</mark> **button of an epoch will open the review screen**. Enter the total budget amount for that epoch, and the app will automatically calculate the payout values to be sent to each recipient.![](<../../../.gitbook/assets/image (8) (2).png>)

6\. Once the budget is set, select the **Payment Category** and enter the **Description** for your reference. Click on the <mark style="color:blue;">**Create Transaction**</mark> button to complete the process.

</details>
