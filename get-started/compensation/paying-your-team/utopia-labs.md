---
description: Paying through Utopia
---

# Utopia Labs

## Step by Step Tutorial

### Before Uploading

1. Download the raw data from Coordinape, and upload that into this Google Sheets template [here.](https://docs.google.com/spreadsheets/d/1z4nDeBKj9Z81se3YIsiaY8JpbnVgz4vI78mUzeRgW6g/edit?usp=sharing)
2. Remove all of the contributors that received 0 GIVE.
3. Remove the “sent” column, which is the column that outlines how much contributors gave to others.
4. Sum up the received column at the bottom
5. Add a column that says “% of budget”
   1. Divide the amount received per contributor by the total sum to get the % of the budget that they’re going to receive.
   2. Add the total budget amount that you planned to pay for this circle/epoch at the bottom of the % of budget column.
6. Add another column that says total received based in USD
   1. Multiply the % of the budget by the total budget amount
   2. By doing this, you know the breakdown of how much the contributor should get paid.

### If the user gets paid in one token, you can move forward with adding two more columns

1. **Amount denominated in **_**(optional) We currently support 5 currencies: USD, CAD, EUR, GBP, AUD**_
   1. This should only be for native token amounts. If you’re paying out in USDC, leave this form field blank.
2.  **Pay-out Token (Required)**

    1. The token you’re paying out in.

    [CSV Payments](https://www.notion.so/a361f457363a4a8fb8eb7a59bd5aaf93)
3. Upload the CSV in Utopia

### IF the contributor gets paid in MULTIPLE tokens, then you’re going go to have to do the following:

1. Create 3 more columns for each token:
   1. Amount
   2. **Amount denominated in** _(optional) We currently support 5 currencies: USD, CAD, EUR, GBP, AUD_
   3. Pay-out Token
   4. Calculate the amounts accordingly.
      1. If you’re paying out in two tokens (assuming you’re paying an equal allocation of each token, divide the total received based in USD by 2
2. Create a new sheets, and copy paste the first table with only the first section of the first token into another sheet.
3. Then, paste the second token amounts UNDERNEATH the first token amount table.
   1. This means that you’re going to have duplicate contributors, wallets, etc.
   2. Again, paste as values only.
   3. In this case tho, if you’re paying out in native tokens, and denominating it based in USD, you would have to add “USD” in the “**Amount denominated in** _(optional) We currently support 5 currencies: USD, CAD, EUR, GBP, AUD” column._

Therefore, if you’re paying out an individual with multiple tokens, then each token requires a new row, meaning duplicate individuals.

Once you have this available, you’re ready to import into Utopia!

{% embed url="https://www.loom.com/share/38d2eb121d044c759555dfdf61c271fa" %}
Utopia Labs Tutorial
{% endembed %}
