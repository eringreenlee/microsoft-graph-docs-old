---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TeamRequestBody();


$requestRequestBodyAdditionalData = [
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->groupsById('group-id')->team()->put($requestRequestBody);


```