---
description: Change Circle Member Settings
---

# Update Members

### Editing User Settings

If you want to change your initial settings for a team member, you can update them in the Admin panel.&#x20;

![The Admin Panel](<../../.gitbook/assets/Screen Shot 2022-05-16 at 6.14.14 PM.png>)

### Member Settings

You can edit the following attributes:

* Starting Tokens
* Admin Permissions&#x20;
* GIVE
* Forced Opt-Out&#x20;
* Opt-Out&#x20;

{% tabs %}
{% tab title="Starting Tokens" %}
By default all users start with 100 GIVE tokens, this can be adjusted as needed when there's no active Epoch [(What's an Epoch)](../get-started/new-coordinape-admins/start-an-epoch.md)
{% endtab %}

{% tab title="Are They Admin" %}
Circles can have multiple admins, but be careful because admins will have full access to your circle settings.&#x20;
{% endtab %}

{% tab title="Can Give" %}
* If Yes, the Contributor will be able to allocate GIVE
* If No, the contributor will not be able to allocate GIVE
{% endtab %}

{% tab title="Forced Opted Out" %}
* If Yes, the contributor will not be able to receive GIVE and will not have the option to Opt-in without admin permission
* If No, the contributor will be able to receive GIVE
{% endtab %}

{% tab title="Opted Out" %}
* If No, the contributor will be able to receive GIVE after they Opt-in in their [Epoch settings](../get-started/new-coordinape-admins/record-contributions.md)
* If Yes, the contributor will have Opted in and immediately eligible to receive give

_Leaving this toggle as NO prevents people from receiving GIVE allocations without logging into Coordinape to allocate to their peers. It may result in them getting fewer allocations if they wait until the end of the epoch to opt-in though_
{% endtab %}
{% endtabs %}

![Edit Member Modal ](<../../.gitbook/assets/Edit User.jpg>)

## Step By Step

* Click the Pencil - Members may be edited by clicking the pencil next to their name.![](<../../.gitbook/assets/User View.jpg>)
* Edit Settings - You can enter their name, starting tokens, admin status, force opt-out, and whether or not they can send GIVE &#x20;
* Force Opt-Out will prevent the user from receiving Give. The user will be alerted to this change via the Telegram Bot and the allocations page. If they have had any give allocated before making that save, it will all be removed, and users who had allocated to them will have to re-allocate to other users.
* ![](<../../.gitbook/assets/Opt Out.jpg>)
* Delete User - You can delete users from the Circle by clicking the trashcan.
