# My Trips - Upcoming trip - Past Driver

Endpoints for upcoming trip (past driver)

## Resource

```
GET /my_trips/handle_action
```

## Parameters


| URI Parameter | Type   | Required | Description |
|:--------------|:-------|:---------|:------------|
| login_hash    | string | yes      |             |
| method     | string |yes       |driver_past             |

## Example

### Request
***

```curl
curl -X GET "http://staging-api.deplacementpeninsule.ca/api/my_trips/handle_action?login_hash=4fee9065a6c6365ddef03cc5102e67fe&method=driver_past"
```

### Response
***

<!--With Login Hash and Method-->
```json
{
  "trip_data": [],
  "status": false
}
```


### Error Responses
***
**Status-Code:** ```200 OK```

<!--
- No Method entered
- With Method driver_past entered
-->

```json
{
  "message": "Please send valid data.",
  "status": ""
}
```
