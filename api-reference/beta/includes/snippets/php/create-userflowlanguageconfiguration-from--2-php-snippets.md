---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UserFlowLanguageConfiguration-idRequestBody();


$requestRequestBodyAdditionalData = [
	"isEnabled" => False,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->languagesById('userFlowLanguageConfiguration-id')->put($requestRequestBody);


```