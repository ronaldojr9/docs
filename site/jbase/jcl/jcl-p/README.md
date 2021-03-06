# jCL P

<PageHeader />

**Tags:**
<badge text='buffer' vertical='middle' />
<badge text='jcl' vertical='middle' />

## Description

This command submits the shell command created in the primary output buffer for execution. It takes the general form:

```
P{P}{H}{Ln}{X}{U}{W}
```

where:

- **P** displays the primary and secondary output buffers. In ROS emulation mode, displays the command and prompts to continue. Normally only used for testing or debugging.
- **H** suppresses (hushes) any terminal output that would normally be displayed. The H and Ln options can be combined as PHLn.
- **Ln** sets an execution lock where n represents a lock number from 0 to 255. The lock is after command has been executed. Any other process attempting to set the same lock is forced to wait. The H and Ln options can be combined as PHLn.
- **X** terminates the program after the command is executed. Cannot be used with any other options.
- **U** specifies that the command is to be submitted for execution by UNIX.
- **W** causes the command to behave like PP when used in a non-ROS emulation.

## Note

> When the P command is executed, control is passed to the shell and only returns when the shell process has been completed. After the P command has been executed, both output buffers are cleared and the stack is turned off.

Commands and data in the secondary output buffer are made available to processes, which require further input. If it is desired to preserve buffer contents when passing control between jCL  programs, use the ( ) or [ ] command instead.

If the PP variants (PP, PPH, and PPLn) are used, the content of both output buffers will be displayed before they are executed and the user will be prompted with a question mark (?). Enter:

- Y   to continue.
- S   to cancel execution but continue the program.
- N   to cancel execution and exit the program.

### Example 1

```
...

HLIST SALES QTR VALUE
P
...
```

Copy the jQL command LIST SALES QTR VALUE to the output buffer and execute it.

### Example 2

```
...

HCOPY SALES ABC
STON
H(SALES.HOLD<
PP
...
```

Place the COPY command in the primary output buffer. Turn the stack on. Put the response to the TO: prompt into the secondary input buffer. Issue the PP command to display the contents of the buffers and prompt for input before continuing.

### Example 3

```
...
Henv | grep EMULATE
...
PU
```

Issue the UNIX grep command.

Back to [jCL.](./../README.md)
  
<PageFooter />