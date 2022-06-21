---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationUser();


$relatedContactsArray = [];

$relatedContacts1 = new RelatedContact();

$relatedContacts1->setDisplayName('Father Time');
$relatedContacts1->setEmailAddress('father@time.com');
$relatedContacts1->setMobilePhone('4251231234');
$relatedContacts1->setRelationship('guardian');
$relatedContacts1->setAccessConsent(True);

$relatedContactsArray []= $relatedContacts1;

$relatedContacts2 = new RelatedContact();

$relatedContacts2->setDisplayName('Mother Nature');
$relatedContacts2->setEmailAddress('mother@nature.co.uk');
$relatedContacts2->setMobilePhone('3251231234');
$relatedContacts2->setRelationship('parent');
$relatedContacts2->setAccessConsent(True);

$relatedContactsArray []= $relatedContacts2;
$requestRequestBody->setRelatedContacts($relatedContactsArray);
 $graphClient->education()->usersById('educationUser-id')->patch($requestRequestBody);


```