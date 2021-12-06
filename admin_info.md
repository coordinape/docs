# Admin Info

![](images/Admin.jpg)

As a Circle Admin, you will be able to edit Circle Settings, Edit Epoch settings, edit your users, and [create new circles](Permissionless\_Circle.md).

### Editing Circle Settings

1. Click the Edit Circle Settings button
2. Fill out the Circle Name, Gift Token Name, Teammate and Allocation page prompts
3. Determine if your Circle will require [vouching](https://docs.coordinape.com/welcome/vouching), and determine the vouching details (How many vouches required, and how long the vouching period is)
4. Determine if users will be opted in by default
5. Link your teams Discord to the [Discord bot](https://docs.coordinape.com/welcome/discord\_bot)

![](<images/Circle Settings.jpg>)

### Editing Epoch Settings

1. Click Edit Epoch Settings
2. Select and Epoch Start and End Date (Recurring feature coming soon™)
3. Click Save
4. You can also delete any Epoch that's not active.

![](<images/Epoch Settings.jpg>) ![](<images/Epoch Settings2.jpg>)

### Editing User Settings

1. After the initial upload of users may be edited by clicking the pencil next to their name![](<images/User View.jpg>)
2. Then you can enter their name, starting tokens, admin status, force opt-out, and whether or not they can send GIVE  ![](<images/Edit User.jpg>)
3. Force Opt Out will prevent the user from receiving Give. The user will be alerted to this change via the Telegram Bot, and on the allocations page. If they have had any give allocated prior to making that save it will all be removed, and users who had allocated to them will have to re-allocate to other users.![](<images/Opt Out.jpg>)
4. You can also delete users from the Circle by clicking the trashcan.

### At the end of an epoch export a CSV of the epoch data for analysis and distribution.

![](images/Export.jpg)Pro tip- If you&#x20;

You can use either the [dispers.app](https://disperse.app) or the Multi distribute in Gnosis safe to distribute you allocations&#x20;

In the Disperse app after you have your csv you can distribute the tokens you wish to allocate by pasting the token address into the token address section

![](<.gitbook/assets/image (2) (1).png>)&#x20;

Pro-tip!

> If you right click and copy the url of the export CSV button and add&#x20;
>
> "\&grant={total\_grant\_amt}"  where {total\_grant\_amt} is replaced by the number of tokens you want to distribute
>
> to the end of your link it will download the csv with the distributed amount already divvied up for you
>
> &#x20;![](.gitbook/assets/image.png)

Then you'll need to take the address and the amount and paste it into the box below.

![](<.gitbook/assets/image (3) (1).png>)

When you're done make sure it looks ok and then click approve and then disperse token

![](<.gitbook/assets/image (1) (1).png>)

### Best Practices

The best practices will vary from team to team. In general we find teams that communicate their goals for using Coordinape to their contributors will have a better experience than teams that start circles without communicating to their users what

**Team Size**&#x20;

Team sizes can range from 2-200+ but we find it's easier to allocate to smaller teams (<20) so the users can have some interaction with most of the members of the team.

**Compensation Amounts**

The amount of compensation for each epoch can vary, it can be zero, it can be infinity.&#x20;

Before our on chain launch there is no escrow feature so the compensation will be distributed by the admin after the epoch ends.

Once on chain, funds for epochs will be escrowed in the Ape Vaults, and automatically made available to claim or distribute at the end of the epoch after the admin approves the distributions.

**Use Cases We've seen**

* Giving to Contributors
* Giving to  Projects
* Giving to other circles

