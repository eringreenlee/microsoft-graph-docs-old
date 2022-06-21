---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new LanguageProficiency();


$requestRequestBody->setAllowedAudiences('organization');
 $graphClient->me()->profile()->languagesById('languageProficiency-id')->patch($requestRequestBody);


```