---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrintTask();


$status = new PrintTaskStatus();
$requestRequestBody->setStatus($status);
$status->setState('completed');
$status->setDescription('completed');

 $graphClient->print()->taskDefinitionsById('printTaskDefinition-id')->tasksById('printTask-id')->patch($requestRequestBody);


```