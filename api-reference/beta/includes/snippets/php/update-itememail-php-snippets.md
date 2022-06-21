---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemEmail();

$requestRequestBody->setDisplayName('Business Email');
$requestRequestBody->setType('work');
 $graphClient->usersById('user-id')->profile()->emailsById('itemEmail-id')->patch($requestRequestBody);


```