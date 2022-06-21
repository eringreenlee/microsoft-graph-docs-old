---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RegistrationRequestBody();

$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.externalMeetingRegistration',
	"allowedRegistrant" => 'everyone',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->post($requestRequestBody);


```