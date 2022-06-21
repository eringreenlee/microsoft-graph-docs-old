---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PhoneAuthenticationMethod-idRequestBody();


$requestRequestBodyAdditionalData = [
	"phoneNumber" => '+1 2065555554',
	"phoneType" => 'mobile',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->me()->authentication()->phoneMethodsById('phoneAuthenticationMethod-id')->put($requestRequestBody);


```