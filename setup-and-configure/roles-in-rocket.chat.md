# Roles in Rocket.Chat

Roles in Rocket.Chat makes managing, controlling, and securing access to resources and features easy in your workspace. A Role can be associated with one or more [**Permissions**](../use-rocket.chat/workspace-administration/permissions.md) allowing users to have different levels of access based on the role assigned to them by the workspace administrator.

As a Rocket.Chat workspace administrator, you can assign certain privileges to users, such as the ability to send messages or manage channels. By assigning roles and permissions, you can control and limit the actions of a user, ensuring that they can only access and perform the actions that they are authorized to do so.

## Categories of Rocket.Chat Roles

### Rocket.Chat Administrator Role

A Rocket.Chat administrator has the `Admin` role, which gives full access to the entire Rocket.Chat workspace. They can manage both [workspace-administration](../use-rocket.chat/workspace-administration/ "mention") and [omnichannel](../use-rocket.chat/omnichannel/ "mention") settings.

### Rocket.Chat User Roles

Rocket.Chat users can have one or more roles, allowing them to perform the various actions granted by the Role's permissions.

| Role          | Description                                                                                                                                                                                                                                                                                   |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `user`        | The user role is the most common in Rocket.Chat. It serves as a standard role for all members of a Rocket.Chat workspace. Users can join [rooms](../use-rocket.chat/user-guides/rooms/), send messages, upload files, and participate in all forms of communication.                          |
| `bot`         | [Bots ](../use-rocket.chat/workspace-administration/settings/bots.md)are automated users that can be programmed to perform specific tasks, such as sending messages, answering questions, and triggering notifications.                                                                       |
| `guest`       | Guest users are non-registered users with access to your Rocket.Chat workspace's public channels.                                                                                                                                                                                             |
| `anonymous`   | Unauthenticated visitors on your Rocket.Chat workspace. Anonymous users do not have a specified username.                                                                                                                                                                                     |
| `app`         | Automated users that are used by Rocket.Chat Apps from the [rocket.chat-marketplace](../extend-rocket.chat-capabilities/rocket.chat-marketplace/ "mention")                                                                                                                                   |
| `Owner`       | A [Channel ](../use-rocket.chat/user-guides/rooms/channels/)owner is a user designated as the owner of a specific channel. The channel owner can manage the channel, including controlling access to joining the channel, editing channel settings, and managing messages within the channel. |
| `Leader`      | A channel Leader gets pinned on the top of a channel and can receive 1:1 messages from other channel users.                                                                                                                                                                                   |
| `Moderator`   | Moderators can manage messages, delete messages, and ban users from a specific channel.                                                                                                                                                                                                       |
| `auditor`     | It allows a user to view and [audit all messages](../use-rocket.chat/message-auditing-log.md)  within the workspace. Users with auditor roles alone cannot send messages.                                                                                                                     |
| `auditor-log` | The `auditor-log` role allows a user to see  [logs about all audited messages](../use-rocket.chat/message-auditing-log.md)  with timestamps and by whom. Users with just the auditor-log role cannot send messages.                                                                           |

### Rocket.Chat Omnichannel Roles

[Omnichannel](../use-rocket.chat/omnichannel/) roles allow users to interact with or manage various Omnichannel features.

| Role               | Description                                                                                                                                                                                                    |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Livechat Agent`   | Live Chat [Agents](../use-rocket.chat/omnichannel/agents.md)handle visitors' inquiries and support requests through [Omnichannel Live Chat](../use-rocket.chat/omnichannel/livechat-widget-installation.md).   |
| `Livechat Manager` | Live Chat [Managers ](../use-rocket.chat/omnichannel/managers.md)can manage Livechat [Agents](../use-rocket.chat/omnichannel/agents.md) and all other [Omnichannel ](../use-rocket.chat/omnichannel/)features. |
| `livechat-monitor` | Users with the `livechat-monitor` role can view and [monitor ](../use-rocket.chat/omnichannel/monitors.md)Live Chat interactions and analytics.                                                                |

{% hint style="info" %}
You can create and manage custom roles with specified permissions tailored to your needs. To learn more, see [#roles](../use-rocket.chat/workspace-administration/permissions.md#roles "mention").
{% endhint %}

### Rocket.Chat Marketplace Roles

Internally, we have two roles for [Rocket.Chat Marketplace](../extend-rocket.chat-capabilities/rocket.chat-marketplace/); one within the publisher and the second within the system. Henceforth, they're known as publisher roles and system roles.

#### Publisher Roles

There are three different roles within a Publisher, which include the following:

* [Owner](roles-in-rocket.chat.md#publisher-owner)
* [Developer](roles-in-rocket.chat.md#publisher-developer)
* [Viewer](roles-in-rocket.chat.md#publisher-viewer)

The Owner role is applied whenever someone creates a publisher. Each of the subsequent roles only applies to people they have invited.

#### Publisher: Owner

The `owner` has permission to manage everything on the publisher dashboard. It includes managing both Apps and other Users.

To change the role of another user,

* Click **Change Role** from the **Actions** dropdown across the user in question
* Select the desired Role to change

#### Publisher: Developer

A user with the `developer` role can read everything and update Apps.

#### Publisher: Viewer

The `viewer` role can read everything but can.t update anything.
