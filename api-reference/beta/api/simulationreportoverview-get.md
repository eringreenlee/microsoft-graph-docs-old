---
title: "Get simulation report overview."
description: "Get report overview for an attack simulation campaign."
author: "Gopal-MSFT"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# Get simulationReportOverview
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get an overview of an attack simulation and training campaign.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | SecurityEvents.Read.All                     |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | SecurityEvents.Read.All                     |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations/{id}/report/overview
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [simulationReportOverview](../resources/simulationreportoverview.md) object in the response body.

## Examples

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_simulationreportoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/overview
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-simulationreportoverview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-simulationreportoverview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-simulationreportoverview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.simulationReportOverview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "microsoft.graph.simulationReportOverview",
  "resolvedTargetsCount": 1,
  "simulationEventsContent": {
    "compromisedRate": 100.0,
    "events": [
      {
        "@odata.type": "microsoft.graph.simulationEvent",
        "eventName": "SuccessfullyDeliveredMail",
        "count": 1
      },
      {
        "@odata.type": "microsoft.graph.simulationEvent",
        "eventName": "ReportedEmail",
        "count": 0
      },
      {
        "@odata.type": "microsoft.graph.simulationEvent",
        "eventName": "EmailLinkClicked",
        "count": 1
      }
    ]
  },
  "trainingEventsContent": {
    "trainingsAssignedUserCount": 1,
    "assignedTrainingsInfos": [
      {
        "@odata.type": "microsoft.graph.assignedTrainingsInfo",
        "assignedUserCount": 1,
        "completedUserCount": 0,
        "displayName": "Sample Training"
      }
    ]
  },
  "recommendedActions": [
    {
      "@odata.type": "microsoft.graph.recommendedAction",
      "actionWebUrl": "https://recommendedSecurityAction.com",
      "title": "Sample Recommended Security Feature",
      "potentialScoreImpact": 5.0
    }
  ]
}
```

