---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendActivityNotificationRequestBody();



$topic = new TeamworkActivityTopic();
$requestRequestBody->setTopic($topic);


$topic->setSource('entityUrl');
$topic->setValue('https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}');

$requestRequestBody->setActivityType('taskCreated');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('New Task Created');

$templateParametersArray = [];

$templateParameters1 = new KeyValuePair();

$templateParameters1->setName('taskId');
$templateParameters1->setValue('Task 12322');

$templateParametersArray []= $templateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
 $graphClient->usersById('user-id')->teamwork()->sendActivityNotification()->post($requestRequestBody);


```