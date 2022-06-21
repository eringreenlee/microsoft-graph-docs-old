---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InternalDomainFederation();

$requestRequestBody->setDisplayName("Contoso name change");
$requestRequestBody->setFederatedIdpMfaBehavior("acceptIfMfaDoneByFederatedIdp");
 $graphClient->domainsById("domain-id")->federationConfigurationById("internalDomainFederation-id")->patch($requestRequestBody);


```