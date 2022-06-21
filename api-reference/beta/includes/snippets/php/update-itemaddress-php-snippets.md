---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemAddress();

$requestRequestBody->setAllowedAudiences("me");
$requestRequestBody->setDisplayName("Secret Hideout");
 $graphClient->usersById("user-id")->profile()->addressesById("itemAddress-id")->patch($requestRequestBody);


```