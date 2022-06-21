---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Site-idRequestBody();

$requestRequestBodyAdditionalData = [
		"value" =>  [
		],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->usersById("user-id")->followedSitesById("site-id")->post($requestRequestBody);


```