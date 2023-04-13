---
description: Streamline Coordinape Tasks with Our Discord Bot
---

# Discord Bot

<details>

<summary>Discord Webhook (Simple Notifications Only)</summary>

### What can the Discord Webhook do?

* Caesar can let your discord know when a users has opted out of a current epoch, and how much give was refunded.

<img src="../../images/Bot Opted Out.jpg" alt="" data-size="original">

* Inform users that an epoch is active

<img src="../../images/Bot Comment (1).jpg" alt="" data-size="original">

* Let users know when the epoch ends

### How to add "Caesar" the discord bot to your teams Discord Channel

1. Click **Edit Channel** on the channel where you want Coordinape notifications to appear. ![](<../../images/Edit Channel.jpg>)
2. Go to I**ntegrations** -> **View Webhook**
3. ![](<../../images/Integrations (1).jpg>)\
   <img src="../../.gitbook/assets/image (12) (2).png" alt="" data-size="original">\\
4. Create **New Webhook** and **Name it** "Coordinape" _(Naming isn't required but it will help your users know where the notifications are coming from)_ click on **Copy Webhook URL**![](<../../images/New Webhook.jpg>)\
   ![](<../../.gitbook/assets/image (3) (1) (2).png>)

4\. Go to Coordinape Circle where you're an Admin and click the **Admin Tab** and scroll to the Integration section and click Edit Webhook

<img src="../../.gitbook/assets/image (57).png" alt="" data-size="original">

5\. **Paste the webhook url** from the Discord bot into text field and **click save**&#x20;

#### BOOM! You now have Caesar helping you keep track of active Epochs, giving you a heads up when users make allocations, and letting you know if a user opts out. We'll be adding features to the bot over time, but in the meantime we hope you enjoy this functionality!

If you appreciate this make sure to let Zashton know!

_You may need to enter developer mode in discord to add the bot_

</details>

## Discord Bot

{% hint style="info" %}
The Bot is currently in beta testing. Please provide any feedback you may have in the Coordinape Discord by going to the **Roles** channel and reacting to the Discord Bot Tester message to get permission to join the Discord Bot Channel. We'll have the bot set up there if you want to test the bot before adding it to your server
{% endhint %}

To add the bot to your server click this link [https://discord.com/api/oauth2/authorize?client\_id=1081300551947538533\&permissions=8\&scope=bot](https://discord.com/api/oauth2/authorize?client\_id=1081300551947538533\&permissions=8\&scope=bot)  and then&#x20;

![](<../../.gitbook/assets/image (6).png>)

Once the bot has been added to your discord use the `/coordinape config` command click **link** account.&#x20;

![](<../../.gitbook/assets/image (3).png>)

once you've linked your account, you will have the option to configure the bot by using the `/Coordinape Config` command and clicking the configure button.

![](<../../.gitbook/assets/image (7).png>)

You can then follow the prompts provided by the bot to finish configuring the bot.&#x20;

{% tabs %}
{% tab title="Add Circles" %}
After adding the Bot to your server you can select which Circles to enable in this server.&#x20;

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
The bot will query your account and will display all Circles you administer. This could include circles across different Orgs so be mindful when selecting circles.
{% endhint %}

1. Click the Dropdown
2. Select the Circles from the drop down
3. Click the input box again
4. Click `Next`

The Bot will create a Channel, and a Role for each Circle in your Discord and then send this message:&#x20;

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

This will ensure the Bot sends the correct alerts and gets the correct commands for each circle in their respective channels

After clicking next navigate to your new channels and click `Link Circle` Button and then click the `Authorize` button

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

This will take you to Coordinape to retrieve your API key for the circle.&#x20;

Once that's complete the bot will ask you if you want it to send alerts for your Circle.&#x20;
{% endtab %}

{% tab title="Enable Alerts" %}
Once you've linked your Circles you will be prompted to set up alerts in your circle. &#x20;

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

#### Alert Descriptions

| Alert                | Description                                                            |
| -------------------- | ---------------------------------------------------------------------- |
| Epoch Start          | Alerts when an Epoch starts                                            |
| Epoch End            | Alerts when an Epoch ends                                              |
| Nomination           | Alert when a user is Nominated for a Circle                            |
| Vouch                | Alert when a user vouches for a Nominee                                |
| Vouch Successful     | Alert when a user is successfully vouched into a circle                |
| Vouch Unsuccessful   | Alert when a user is not successfully vouched into a circle            |
| User Added to Circle | Alert when a user is added to a circle                                 |
| User Leaves a Circle | Alert when a User leaves a Circle                                      |
| User Opts out        | Alert when a User opts out of receiving Give from other Circle Members |
{% endtab %}
{% endtabs %}

### Contributions

You can now add contributions directly from within Discord!&#x20;

It's as simple as typing `/Coordinape Contribute` in Discord and then entering the contribution you made.&#x20;

In this MVP version each Coordinape Circle is linked 1-1 to a Discord channel, so you must enter your contributions in a linked channel for the command to work correctly

\
