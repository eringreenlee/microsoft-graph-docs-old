---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new TeamworkTag();
$requestBody->setDisplayName('Finance');



$graphServiceClient->teamsById('team-id')->tagsById('teamworkTag-id')->patch($requestBody);


```