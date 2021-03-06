# Rating Received

This endpoint is used for Viewing Ratings Received

## Resource

```
POST /ratings/rating_received
```

## Parameters


| URI Parameter | Type   | Required | Description     |
|:--------------|:-------|:---------|:----------------|
| login_hash    | string | yes      | <user hash key> |
| site_lang     | string | yes      | en              |



## Example

### Request
***

```curl
curl -X POST "http://staging-api.deplacementpeninsule.ca/api/ratings/rating_received?login_hash=4fee9065a6c6365ddef03cc5102e67fe&site_lang=en"
```

### Response
***

**Status-Code:**

```

```


### Error Responses
***
<!--
- No Login Hash
- With Login Hash and Site Lang
-->
**Status-Code:** ```200 OK```


```json
{
  "message": "Please log in with us. Don't have an account sign up now!",
  "status": false
}
```

<!--No Site Language-->
**Status-Code:** ```404 Not Found```


```
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>404 Not Found</title>
</head><body>
<h1>Not Found</h1>
<p>The requested URL /fr/api/message/unread was not found on this server.</p>
</body></html>
```
