---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewEvent()
subject := "Let's go for lunch"
requestBody.SetSubject(&subject) 
body := graphmodels.NewItemBody()
contentType := graphmodels.HTML_BODYTYPE 
body.SetContentType(&contentType) 
content := "Does mid month work for you?"
body.SetContent(&content) 
requestBody.SetBody(body)
start := graphmodels.NewDateTimeTimeZone()
dateTime := "2019-03-15T12:00:00"
start.SetDateTime(&dateTime) 
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone) 
requestBody.SetStart(start)
end := graphmodels.NewDateTimeTimeZone()
dateTime := "2019-03-15T14:00:00"
end.SetDateTime(&dateTime) 
timeZone := "Pacific Standard Time"
end.SetTimeZone(&timeZone) 
requestBody.SetEnd(end)
location := graphmodels.NewLocation()
displayName := "Harry's Bar"
location.SetDisplayName(&displayName) 
requestBody.SetLocation(location)


 := graphmodels.New()
additionalData := map[string]interface{}{
emailAddress := graphmodels.New()
address := "adelev@contoso.onmicrosoft.com"
emailAddress.SetAddress(&address) 
name := "Adele Vance"
emailAddress.SetName(&name) 
	.SetEmailAddress(emailAddress)
	"type" : "required", 
}
.SetAdditionalData(additionalData)

attendees := []graphmodels.Objectable {
	,

}
requestBody.SetAttendees(attendees)
transactionId := "7E163156-7762-4BEB-A1C6-729EA81755A7"
requestBody.SetTransactionId(&transactionId) 

result, err := graphClient.Me().CalendarsById("calendar-id").Events().Post(requestBody)


```