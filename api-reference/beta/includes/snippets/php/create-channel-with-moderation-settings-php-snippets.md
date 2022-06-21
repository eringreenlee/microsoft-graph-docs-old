---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();

$requestRequestBody->setDisplayName("TestChannelModeration");
$requestRequestBody->setDescription("Test channel moderation.");
$requestRequestBody->setMembershipType("standard");

$moderationSettings = new ChannelModerationSettings();
$requestRequestBody->setModerationSettings($moderationSettings);
$moderationSettings->setUserNewMessageRestriction("everyoneExceptGuests");
$moderationSettings->setReplyRestriction("everyone");
$moderationSettings->setAllowNewMessageFromBots(True);
$moderationSettings->setAllowNewMessageFromConnectors(True);

$result =  $graphClient->teamsById("team-id")->channels()->post($requestRequestBody);


```