---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CopyToSectionGroupRequestBody();


$requestRequestBody->setId('id-value');
$requestRequestBody->setGroupId('groupId-value');
$requestRequestBody->setRenameAs('renameAs-value');
$result =  $graphClient->me()->onenote()->sectionsById('onenoteSection-id')->copyToSectionGroup()->post($requestRequestBody);


```