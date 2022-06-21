---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcOrganizationSettings();


$requestRequestBody->setUserAccountType('standardUser');
$requestRequestBody->setOsVersion('windows11');

$windowsSettings = new CloudPcWindowsSettings();
$requestRequestBody->setWindowsSettings($windowsSettings);


$windowsSettings->setLanguage('en-US');

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.cloudPcOrganizationSettings',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->deviceManagement()->virtualEndpoint()->organizationSettings()->patch($requestRequestBody);


```