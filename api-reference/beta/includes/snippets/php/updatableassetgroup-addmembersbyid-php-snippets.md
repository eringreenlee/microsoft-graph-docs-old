---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AddMembersByIdRequestBody();

$requestRequestBody->setIds( [
'String','String','String',],
$requestRequestBody->setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');
 $graphClient->admin()->windows()->updates()->updatableAssetsById('updatableAsset-id')->addMembersById()->post($requestRequestBody);


```