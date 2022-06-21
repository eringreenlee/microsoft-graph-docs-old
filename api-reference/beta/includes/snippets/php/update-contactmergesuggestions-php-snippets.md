---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ContactMergeSuggestions();

$requestRequestBody->setIsEnabled(False);
 $graphClient->me()->settings()->contactMergeSuggestions()->patch($requestRequestBody);


```