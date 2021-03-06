# JExecuteResults (jrclient API)

<PageHeader />

## Class JExecuteResults

com.jbase.jrcs.JExecuteResults

``` java
public final class JExecuteResults
extends Object
```

Contains results of jCL/jQL command execution

## Constructor Summary

| Modifier | Constructor and Description |
| --- | --- |
| protected | JExecuteResults(String capturing, [JCapture](./../jcapture-jrclient-api "class in com.jbase.jrcs") captureObj, String returning, [JSelectList](./../jselectlist-jrclient-api "class in com.jbase.jrcs") returnList) |

## Method Summary

| Modifier and Type |  Method |  Description |
| --- | --- | --- |
| [JCapture](./../jcapture-jrclient-api "class in com.jbase.jrcs") | getCapture() | Returns an incremental fetch capture object or null if there is no capture object |
| String | getCaptureString() | the capture string or null if there is no capture string |
| [JSelectList](./../jselectlist-jrclient-api "class in com.jbase.jrcs") | getReturnList() | Retrieves the select list generated by command |
| String | getReturnString() | Retrieves the return string generated by command or null if there is no return string |

## Methods inherited from class java.lang.Object

`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

### Constructor Detail

#### **JExecuteResults**

``` java
protected JExecuteResults(String capturing, JCapture captureObj, String returning, JSelectList returnList)
```

### Method Detail

#### getCaptureString

``` java
public String getCaptureString()
```

Returns the capture string or null if there is no capture string

Returns: Capture string or null.

#### getCapture

``` java
public JCapture getCapture()
```

Returns an incremental fetch capture object or null if there is no capture object.

Returns: JCapture object used for fetching execution capture incrementally

#### getReturnString

``` java
public String getReturnString()
```

Retrieves the return string generated by command or null if there is no return string.

Returns: Return string

#### getReturnList

``` java
public JSelectList getReturnList()
```

Retrieves the select list generated by command.

Returns: JSelectList object referencing the resulting select list

Back to [jRCS java API](./../README.md)

  
<PageFooter />
