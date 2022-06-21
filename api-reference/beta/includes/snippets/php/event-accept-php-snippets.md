---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AcceptRequestBody();

$requestRequestBody->setComment("comment-value");
$requestRequestBody->setSendResponse(True);
 $graphClient->me()->eventsById("event-id")->accept()->post($requestRequestBody);


```