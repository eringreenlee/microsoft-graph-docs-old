---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewGetByIdsPostRequestBody()
ids := []String {
	"84b80893-8749-40a3-97b7-68513b600544",
	"5d6059b6-368d-45f8-91e1-8e07d485f1d0",

}
requestBody.SetIds(ids)
types := []String {
	"user",

}
requestBody.SetTypes(types)

result, err := graphClient.DirectoryObjects().GetByIds().Post(requestBody)


```