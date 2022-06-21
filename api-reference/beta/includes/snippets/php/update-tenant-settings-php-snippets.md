---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Settings();


$requestRequestBody->setDeletedUserPersonalSiteRetentionPeriodInDays(365);
$requestRequestBody->setExcludedFileExtensionsForSyncApp( [
'.mp3',],
$requestRequestBody->setImageTaggingOption('enhanced');
$requestRequestBody->setIsSitesStorageLimitAutomatic(False);
$requestRequestBody->setIsSyncButtonHiddenOnPersonalSite(False);
$requestRequestBody->setIsUnmanagedSyncAppForTenantRestricted(False);
$requestRequestBody->setPersonalSiteDefaultStorageLimitInMB(120000);
 $graphClient->admin()->sharepoint()->settings()->patch($requestRequestBody);


```