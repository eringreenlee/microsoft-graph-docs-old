---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChangePasswordRequestBody();

$requestRequestBody->setCurrentPassword("xWwvJ]6NMw+bWH-d");
$requestRequestBody->setNewPassword("0eM85N54wFxWwvJ]");
 $graphClient->me()->changePassword()->post($requestRequestBody);


```