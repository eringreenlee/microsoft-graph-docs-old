---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BundlesRequestBody();

$requestRequestBodyAdditionalData = [
		"name" => "Just some files",
		"@microsoft.graph.conflictBehavior" => "rename",
		"children" =>  [
		],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->drive()->bundles()->post($requestRequestBody);


```