---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TranslateExchangeIdsRequestBody();

$requestRequestBody->setInputIds( [
'{rest-formatted-id-1}','{rest-formatted-id-2}',],
$requestRequestBody->setSourceIdType('restId');
$requestRequestBody->setTargetIdType('restImmutableEntryId');
$result =  $graphClient->me()->translateExchangeIds()->post($requestRequestBody);


```