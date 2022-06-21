---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SectionGroupsRequestBody();

$requestRequestBodyAdditionalData = [
	"displayName" => 'Section group name',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->me()->onenote()->sectionGroupsById('sectionGroup-id')->sectionGroups()->post($requestRequestBody);


```