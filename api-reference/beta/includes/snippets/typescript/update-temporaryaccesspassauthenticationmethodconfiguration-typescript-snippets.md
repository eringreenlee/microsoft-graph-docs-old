---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationMethodConfiguration = {
	additionalData : {
		"@odata.type" : "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
		isUsableOnce : true,
	},
};

const result = async () => {
	await graphServiceClient.policies.authenticationMethodsPolicy.authenticationMethodConfigurationsById("authenticationMethodConfiguration-id").patch(requestBody);
}


```