---
title: "Get applicationTemplate"
description: "Retrieve the properties and relationships of applicationtemplate object."
localization_priority: Normal
author: "luleonpla"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get applicationTemplate

Namespace: microsoft.graph

Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | None. |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | None. |

Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## Optional query parameters

You can use a `$select` query parameter to specify only the properties you need for best performance. The **id** property is always returned. 

For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name      |Description|
|:----------|:----------|
| Authorization | Bearer {code} |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.

## Examples

### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applicationTemplates/cd3ed3de-93ee-400b-8b19-b61ef44a0f29
```

### Response

The following is an example of the response.

> [!NOTE]
> The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{	
  "id": "cd3ed3de-93ee-400b-8b19-b61ef44a0f29",
  "displayName": "Salesforce",
  "homePageUrl": "https://www.microsoft.com/",
  "supportedSingleSignOnModes": [
      "password",
      "saml",
      "external"
  ],
  "supportedProvisioningTypes": [
      "sync"
  ],
  "logoUrl": "https://az495088.vo.msecnd.net/app-logo/salesforce.com_215.png",
  "categories": [
      "crm",
      "topApps"
  ],
  "publisher": "Microsoft"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


