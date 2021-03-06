# REWIND

<PageHeader />

## Description

The **REWIND** statement will issue a rewind command to the device attached to the specified channel. It takes the general form:

```
REWIND{ON expression} THEN|ELSE statements
```

Where:

**expression**, if specified, should evaluate to an integer in the range 0 to 9. Default is 0.

## Note

> If the statement fails to issue the rewind then any statements associated with the **ELSE** clause are executed. If the statement successfully issues the rewind command then the **statements** associated with any **THEN** clause are executed. Either or both of the **THEN** and **ELSE** clauses must be specified with the statement.
>
> If the statement fails then the reason for failure can be determined via the value of [SYSTEM(0)](./../system-functions) as follows:
>
>
> | Value | Meaning |
> | --- | --- |
> | 1 | There is no media attached to the channel |
> | 2 | An end of file mark was found |

Go back  to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
