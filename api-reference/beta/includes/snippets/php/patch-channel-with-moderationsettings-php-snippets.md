---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();

$requestRequestBody->setDisplayName("UpdateChannelModeration");
$requestRequestBody->setDescription("Update channel moderation.");

$moderationSettings = new ChannelModerationSettings();
$requestRequestBody->setModerationSettings($moderationSettings);
$moderationSettings->setUserNewMessageRestriction("moderators");
$moderationSettings->setReplyRestriction("everyone");
$moderationSettings->setAllowNewMessageFromBots(True);
$moderationSettings->setAllowNewMessageFromConnectors(True);

 $graphClient->teamsById("team-id")->channelsById("channel-id")->patch($requestRequestBody);


```