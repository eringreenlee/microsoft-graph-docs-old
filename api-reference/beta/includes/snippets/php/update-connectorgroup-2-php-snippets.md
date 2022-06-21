---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConnectorGroup();

$requestRequestBody->setName("name-value");
$requestRequestBody->setRegion("region-value");
 $graphClient->onPremisesPublishingProfilesById("onPremisesPublishingProfile-id")->connectorGroupsById("connectorGroup-id")->patch($requestRequestBody);


```