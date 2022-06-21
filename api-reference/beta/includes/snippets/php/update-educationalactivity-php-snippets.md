---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationalActivity();



$institution = new InstitutionData();
$requestRequestBody->setInstitution($institution);



$location = new PhysicalAddress();
$institution->setLocation($location);


$location->setType('business');
$location->setPostOfficeBox(null);
$location->setStreet('12000 E Prospect Rd');
$location->setCity('Fort Collins');
$location->setState('Colorado');
$location->setCountryOrRegion('USA');
$location->setPostalCode('80525');


 $graphClient->me()->profile()->educationalActivitiesById('educationalActivity-id')->patch($requestRequestBody);


```