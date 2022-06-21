---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EmailAuthenticationMethod-idRequestBody();


$requestRequestBodyAdditionalData = [
	"emailAddress" => 'kim@contoso.com',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->usersById('user-id')->authentication()->emailMethodsById('emailAuthenticationMethod-id')->put($requestRequestBody);


```