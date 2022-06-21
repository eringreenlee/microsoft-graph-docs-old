---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SchemaRequestBody();


$requestRequestBodyAdditionalData = [
	"directories" =>  [
	],
	"synchronizationRules" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->schema()->put($requestRequestBody);


```