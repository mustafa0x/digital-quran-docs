# Errors

* If the server returned status code not equals 200 then an error occurred.
* You should always check that the response is a valid JSON.

If an error occurs during the request, the server will return the response in the following format:

```javascript
{
    "error": {
        "code": "ERROR_CODE",
        "message": "Message with error description."
    }
}
```

The response status code will be 200, not 4xx or 5xx, because it's not a REST API. If the server returned a response with code 4xx or 5xx it means that something went wrong and the server couldn't handle an error correctly, so the response may be an invalid JSON.

You have to handle both cases: if the response status code does not equals 200 and if the response contains the field "error".

Every endpoint may have it's own error codes but there are also common error codes.

## Common error codes

**UNKNOWN\_ERROR**

Unknown error occurred. Typically a server bug.

**NOT\_FOUND**

Endpoint not found. Check request URL is correct.

**RESOURCE\_NOT\_FOUND**

Requested resource \(translation, for example\) not found.

**METHOD\_NOT\_ALLOWED**

The request method is not POST.

**INVALID\_REQUEST**

1. "Content-Type" header is not provided or it not equals "application/json".
2. The request is not a valid JSON.

**ACCESS\_TOKEN\_NOT\_PROVIDED**

Access token is not provided.

**INVALID\_ACCESS\_TOKEN**

Access token is invalid.

**TOO\_MANY\_REQUESTS**

Too many requests. Check out [limits](limits.md) for more information.

**LANGUAGE\_NOT\_PROVIDED**

"Language" header is not provided.

**UNKNOWN\_LANGUAGE**

Unknown language code provided. See the [list of available languages](https://github.com/quranacademy/digital-quran-docs/tree/5ac35f82b33be44b98843418794dc47bf7dcdf68/api/available-languages.md).

**INVALID\_PARAMETERS**

Invalid parameter\(s\) provided.

This error means that some of the passed parameters are invalid. In response, you will get `validation_errors` field with validation error messages.

Example:

```javascript
{
    "error": {
        "code": "INVALID_PARAMETERS",
        "message": "Some of passed parameters are invalid"
    },
    "validation_errors": {
        "surah": "Surah number must be an integer from 1 to 114"
    },
}
```

**INTERNAL\_SERVER\_ERROR**

Internal server error occurred. Typically a server bug.

