---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CrossTenantAccessPolicyConfigurationPartner();


$requestRequestBody->setTenantId('3d0f5dec-5d3d-455c-8016-e2af1ae4d31a');

$b2bDirectConnectOutbound = new CrossTenantAccessPolicyB2BSetting();
$requestRequestBody->setB2bDirectConnectOutbound($b2bDirectConnectOutbound);



$usersAndGroups = new CrossTenantAccessPolicyTargetConfiguration();
$b2bDirectConnectOutbound->setUsersAndGroups($usersAndGroups);


$usersAndGroups->setAccessType('blocked');
$targetsArray = [];

$targets1 = new CrossTenantAccessPolicyTarget();

$targets1->setTarget('6f546279-4da5-4b53-a095-09ea0cef9971');
$targets1->setTargetType('group');

$targetsArray []= $targets1;
$usersAndGroups->setTargets($targetsArray);



$b2bDirectConnectInbound = new CrossTenantAccessPolicyB2BSetting();
$requestRequestBody->setB2bDirectConnectInbound($b2bDirectConnectInbound);



$applications = new CrossTenantAccessPolicyTargetConfiguration();
$b2bDirectConnectInbound->setApplications($applications);


$applications->setAccessType('allowed');
$targetsArray = [];

$targets1 = new CrossTenantAccessPolicyTarget();

$targets1->setTarget('Office365');
$targets1->setTargetType('application');

$targetsArray []= $targets1;
$applications->setTargets($targetsArray);


$result =  $graphClient->policies()->crossTenantAccessPolicy()->partners()->post($requestRequestBody);


```