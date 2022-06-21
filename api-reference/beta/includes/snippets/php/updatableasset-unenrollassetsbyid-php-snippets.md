---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnenrollAssetsByIdRequestBody();

$requestRequestBody->setUpdateCategory('feature');
$requestRequestBody->setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');
$requestRequestBody->setIds( [
'String','String','String',],
 $graphClient->admin()->windows()->updates()->updatableAssets()->unenrollAssetsById()->post($requestRequestBody);


```