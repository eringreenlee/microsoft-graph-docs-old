---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewMessage()
subject := "Annual review"
requestBody.SetSubject(&subject) 
body := graphmodels.NewItemBody()
contentType := graphmodels.HTML_BODYTYPE 
body.SetContentType(&contentType) 
content := "You should be proud!"
body.SetContent(&content) 
requestBody.SetBody(body)


recipient := graphmodels.NewRecipient()
emailAddress := graphmodels.NewEmailAddress()
address := "rufus@contoso.com"
emailAddress.SetAddress(&address) 
recipient.SetEmailAddress(emailAddress)

toRecipients := []graphmodels.Recipientable {
	recipient,

}
requestBody.SetToRecipients(toRecipients)


extension := graphmodels.NewExtension()
"@odata.type" := "microsoft.graph.openTypeExtension"
extension.Set"@odata.type"(&"@odata.type") 
additionalData := map[string]interface{}{
	"extensionName" : "Com.Contoso.Referral", 
	"companyName" : "Wingtip Toys", 
	"expirationDate" : "2015-12-30T11:00:00.000Z", 
	"dealValue" : int32(10000) , 
}
extension.SetAdditionalData(additionalData)

extensions := []graphmodels.Extensionable {
	extension,

}
requestBody.SetExtensions(extensions)

result, err := graphClient.Me().Messages().Post(requestBody)


```