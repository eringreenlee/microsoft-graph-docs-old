---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RejectRequestBody();


$requestRequestBody->setReason('none');
 $graphClient->communications()->callsById('call-id')->reject()->post($requestRequestBody);


```