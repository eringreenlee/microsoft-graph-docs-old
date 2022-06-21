---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SkillProficiency();

$requestRequestBody->setCategories( [
"Professional",],
$requestRequestBody->setProficiency("advancedProfessional");
 $graphClient->me()->profile()->skillsById("skillProficiency-id")->patch($requestRequestBody);


```