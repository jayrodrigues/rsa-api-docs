# Settings - Vehicle - Load Models

Endpoint to load Vehicle Makes when adding/editing a Vehicle.

## Resource

```
GET /settings/load_models
```

## Parameters


Name              	| Type   	| Description
:------------------|:----------	|:--------------------
login_hash			|string		|**[required]** <user hash key>
year  |string|**[required]**
make_id | int|


## Example

### Request
***

```curl
curl -X GET "http://staging-api.deplacementpeninsule.ca/api/settings/load_models?login_hash=4fee9065a6c6365ddef03cc5102e67fe&year=2015&make_id=1"
```

### Response
***

**Status-Code:** ```200 OK```

```json
{
  "models": [
    {
      "value": "2735",
      "label": "ILX"
    },
    {
      "value": "2736",
      "label": "ILX HYBRID"
    },
    {
      "value": "3008",
      "label": "MDX SH-AWD"
    },
    {
      "value": "2737",
      "label": "RDX AWD"
    },
    {
      "value": "2860",
      "label": "RLX"
    },
    {
      "value": "3009",
      "label": "RLX HYBRID"
    },
    {
      "value": "3010",
      "label": "TLX"
    },
    {
      "value": "3011",
      "label": "TLX SH-AWD"
    }
  ],
  "status": true
}
```


### Error Responses
***

**Status-Code:** ```200 OK```


```json
{
  "message": "Please send valid data.",
  "status": false,
  "makes": []
}
```


**Status-Code:** ```200 OK```


```json
{
  "models": [],
  "status": true
}
```