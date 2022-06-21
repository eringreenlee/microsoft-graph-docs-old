---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProvider-idRequestBody();

$requestRequestBodyAdditionalData = [
		"@odata.id" => "https://graph.microsoft.com/beta/identityProviders/{id}",
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->identity()->b2xUserFlowsById("b2xIdentityUserFlow-id")->identityProvidersById("identityProvider-id")->post($requestRequestBody);


```