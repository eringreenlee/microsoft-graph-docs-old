---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingCustomQuestion();


$requestRequestBody->setDisplayName('What is your age?');
$requestRequestBody->setAnswerInputType('text');
$requestRequestBody->setAnswerOptions( [
],
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingCustomQuestion',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->bookingBusinessesById('bookingBusiness-id')->customQuestionsById('bookingCustomQuestion-id')->patch($requestRequestBody);


```