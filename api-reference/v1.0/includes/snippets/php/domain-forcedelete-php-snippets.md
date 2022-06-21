---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DisableUserAccountsRequestBody();

$requestRequestBody->setDisableUserAccounts(True);
 $graphClient->domainsById("domain-id")->forceDelete()->post($requestRequestBody);


```