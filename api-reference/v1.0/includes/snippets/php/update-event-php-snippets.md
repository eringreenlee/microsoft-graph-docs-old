---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Event();


$requestRequestBody->setOriginalStartTimeZone('originalStartTimeZone-value');
$requestRequestBody->setOriginalEndTimeZone('originalEndTimeZone-value');

$responseStatus = new ResponseStatus();
$requestRequestBody->setResponseStatus($responseStatus);


$responseStatus->setResponse('');
$responseStatus->setTime(new DateTime("datetime-value"));

$requestRequestBody->setRecurrence(null);
$requestRequestBody->setReminderMinutesBeforeStart(99);
$requestRequestBody->setIsOnlineMeeting(True);
$requestRequestBody->setOnlineMeetingProvider('teamsForBusiness');
$requestRequestBody->setIsReminderOn(True);
$requestRequestBody->setHideAttendees(False);
$requestRequestBody->setCategories( [
'Red category',],
 $graphClient->me()->eventsById('event-id')->patch($requestRequestBody);


```