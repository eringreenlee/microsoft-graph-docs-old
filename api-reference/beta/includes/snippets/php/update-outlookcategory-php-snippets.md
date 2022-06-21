---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookCategory();

$requestRequestBody->setColor('preset15');
 $graphClient->me()->outlook()->masterCategoriesById('outlookCategory-id')->patch($requestRequestBody);


```