---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExportRequestBody();

$requestRequestBody->setOutputName("Export reviewset query via API");
$requestRequestBody->setDescription("Export for the Contoso investigation 2");
$requestRequestBody->setExportOptions("originalFiles,fileInfo,tags");
$requestRequestBody->setExportStructure("directory");
 $graphClient->security()->cases()->ediscoveryCasesById("ediscoveryCase-id")->reviewSetsById("ediscoveryReviewSet-id")->queriesById("ediscoveryReviewSetQuery-id")->export()->post($requestRequestBody);


```