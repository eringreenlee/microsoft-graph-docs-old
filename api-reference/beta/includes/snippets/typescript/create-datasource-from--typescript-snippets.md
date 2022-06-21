---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DataSource = {
	additionalData : {
		"@odata.type" : "microsoft.graph.security.siteSource",
		site : {
			webUrl : "https://contoso.sharepoint.com/sites/SecretSite",
		},
	},
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").searchesById("ediscoverySearch-id").additionalSources.post(requestBody);
}


```