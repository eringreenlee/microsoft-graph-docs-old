---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReprovisionRequestBody();


$requestRequestBody->setUserAccountType('administrator');
$requestRequestBody->setOsVersion('windows10');
 $graphClient->deviceManagement()->virtualEndpoint()->cloudPCsById('cloudPC-id')->reprovision()->post($requestRequestBody);


```