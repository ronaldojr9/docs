# curlUseMemory

<PageHeader />

This function is typically used to reset the ***curlHandle*** if [curlUseFile](../curlUseFile#heading) was previously used.

## Synax:

***result_code*** = **curlUseMemory**(***curlHandle***)

where:

| Variable | Type | Description |
|--|--|--|
***result_code*** | integer | result code
***curlHandle*** | var | a [jCURL](../../jcurl) handle generated by [curlInit](../curlinit)

## Example

```
INCLUDE JBCCURL.h
rc = curlInit(curlHandle)
... perform curl operations with curlHandle
rc = curlUseMemory(curlHandle)
rc = curlExec(curlHandle, result, headers)
...
```

Click here [$ftp class](../#ftpclass-jabba) for a practical use of curlUseMemory.

see also [curlUseVar](../curlUseVar) and [curlUseFile](../curlUseFile)

Back to [jCurl.](./../README.md)

  
<PageFooter />
