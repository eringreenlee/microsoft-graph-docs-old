---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReplyAllRequestBody();

$requestRequestBody->setComment('comment-value');
 $graphClient->me()->messagesById('message-id')->replyAll()->post($requestRequestBody);


```