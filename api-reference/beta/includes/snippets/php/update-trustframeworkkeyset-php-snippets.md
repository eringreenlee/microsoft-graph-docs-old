---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TrustFrameworkKeySet-idRequestBody();

$requestRequestBodyAdditionalData = [
	"keys" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->trustFramework()->keySetsById('trustFrameworkKeySet-id')->put($requestRequestBody);


```