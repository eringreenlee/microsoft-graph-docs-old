---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationRubric();


$requestRequestBody->setDisplayName('Example Credit Rubric after display name patch');
 $graphClient->education()->me()->rubricsById('educationRubric-id')->patch($requestRequestBody);


```