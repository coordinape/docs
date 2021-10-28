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

1. After the initial upload of users may be edited by clicking the pencil next to their name

![](<images/User View.jpg>)

1. Then you can enter their name, starting tokens, admin status, force opt-out, and whether or not they can send GIVE

![](<images/Edit User.jpg>)

1. Force Opt Out will prevent the user from receiving Give. The user will be alerted to this change via the Telegram Bot, and on the allocations page. If they have had any give allocated prior to making that save it will all be removed, and users who had allocated to them will have to re-allocate to other users.

![](<images/Opt Out.jpg>)

1. You can also delete users from the Circle by clicking the trashcan.

### You can also export a CSV of the epoch data for analysis.

![](images/Export.jpg)

### Best Practices

The best practices will vary from team to team. In general we find teams that communicate their goals for using Coordinape to their contributors will have a better experience than teams that start circles without communicating to their users what

**Team Size **

Team sizes can range from 2-200+ but we find it's easier to allocate to smaller teams (<20) so the users can have some interaction with most of the members of the team.

**Compensation Amounts**

The amount of compensation for each epoch can vary, it can be zero, it can be infinity.&#x20;

Before our on chain launch there is no escrow feature so the compensation will be distributed by the admin after the epoch ends.

Once on chain, funds for epochs will be escrowed in the Ape Vaults, and automatically made available to claim or distribute at the end of the epoch after the admin approves the distributions.

**Use Cases We've seen**

* Giving to Contributors
* Giving to  Projects
* Giving to other circles

