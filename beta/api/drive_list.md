# List drives

Retrieve a list of drive objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /drives
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [drive](../resources/drive.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->
```http
GET https://graph.microsoft.com/v1.0/drives
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
Content-type: application/json
Content-length: 579

{
  "value": [
    {
      "id": "id-value",
      "driveType": "driveType-value",
      "owner": {
        "application": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "device": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "user": {
          "displayName": "displayName-value",
          "id": "id-value"
        }
      },
      "quota": {
        "deleted": 99,
        "remaining": 99,
        "state": "state-value",
        "total": 99,
        "used": 99
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->