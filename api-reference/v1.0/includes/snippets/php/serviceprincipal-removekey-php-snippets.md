---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RemoveKeyRequestBody();


$requestRequestBody->setKeyId('f0b0b335-1d71-4883-8f98-567911bfdca6');
$requestRequestBody->setProof('eyJ0eXAiOiJ...');
 $graphClient->servicePrincipalsById('servicePrincipal-id')->removeKey()->post($requestRequestBody);


```