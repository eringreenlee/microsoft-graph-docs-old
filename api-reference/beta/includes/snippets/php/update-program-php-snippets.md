---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Program();

$requestRequestBody->setDisplayName('testprogram3 new name');
 $graphClient->programsById('program-id')->patch($requestRequestBody);


```