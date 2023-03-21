---
description: How to integrate Coordinape with Hedgey.finance
---

# Hedgey

Hedgey's Contributor Rewards allow DAOs and tokenized communities to distribute locked tokens to their core contributors, while giving recipients a unique NFT which represents ownership of the locked tokens they've received. These NFTs can retain token voting rights, give access to gated communities and provide a host of other benefits.

**Notes:**

* **Supported networks:** Ethereum only with Coordinape now

{% hint style="info" %}
Hedgey also supports Polygon, Avalanche, Harmony, Fantom, Gnosis Chain, Celo, Boba, Arbitrum One and Optimism so this integration could flourish across chains soon!&#x20;
{% endhint %}

* **Supported tokens:** Any standard token used for contributor rewards.
* **GitHub documentation for Contributor Rewards can be found** [**here**](https://github.com/hedgey-finance/NFT\_OTC\_Core)**.**&#x20;
* **Audit for Contributor Rewards can be found** [**here**](https://github.com/hedgey-finance/NFT\_OTC\_Core/blob/main/audits/Hedgey\_31032022\_SCAudit\_Report\_2.pdf)**.**&#x20;

If you'd like to know more about Hedgy click [here](https://hedgey.finance)

## Enable Coordinape Integration

1. Navigate to the Admin Tab and Scroll to the [Integrations ](./)section
   1. ![](<../../.gitbook/assets/image (33).png>)
2. Select your settings and click Save Hedgey Settings
   1. ![](<../../.gitbook/assets/image (50).png>)

### Utilize Hedgey Integration

After you've enabled the integration you can now use fund any completed epoch with locked tokens.&#x20;

1. Go to your Circle Overview, select a Epoch that hasn't been paid out yet, and click Review/Export
   1. ![](<../../.gitbook/assets/image (21).png>)
2. Select Hedgey as your CoVault Source
   1. ![](<../../.gitbook/assets/image (23).png>)
3. Add the token address you of the token you want to distribute, the amount you want to pay, the lock period, transferability, and then click submit for Distribution.
   1. ![](<../../.gitbook/assets/image (18).png>)
4. There will be an additional Signature required to batch mint the NFT for the recipients of the Distributions. This NFT and the locked tokens can be claimed on the bottom of the Claims page
   1. ![](<../../.gitbook/assets/image (1) (7).png>)
5. Clicking on View Hedgeys button will take you to Hedgey.Finance to view the NFT's and details about your NFT's
   1. ![](<../../.gitbook/assets/image (16).png>)
   2. ![](<../../.gitbook/assets/image (8).png>)
6. When the Locking period has passed the tokens will be unlocked to do what you wish with them
