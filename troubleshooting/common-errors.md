# Error response

All response bodies from Dialex come with a `status` field containing the value of a standard HTTP response code along with an `error` message.

```
{
    "status": 429,
    "error": "Out of API requests"
}
```

Error codes used by Dialex. Note that conventional HTTP status codes do apply.

| Status | Info |
| :--- | :--- |
| 200 | Operation successful |
| 401 | Incorrect authorization data or unauthorization |
| 429 | Excessive calls to API or exceeded account API call limit. Check error message for more information. |
| 5XX | Server error |



