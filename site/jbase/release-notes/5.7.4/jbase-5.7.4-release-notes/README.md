# jBASE 5.7.4 Release Notes

<PageHeader />

This release includes various internal bug fixes and the following enhancements and patches:

## Patches

- [PN5\_60894](./../pn5_60894/README.md) - **listf -xml** does not work on Linux
- [PN5\_60899](./../pn5_60899/README.md) - New options for jbase\_agent: -d,-a,-J[dDpr]
- [PN5\_60900](./../pn5_60900/README.md) - Add extensions to Dynamic Objects per RFC 7159
- [PN5\_60902](./../pn5_60902/README.md) - Distributed Files: Add new error messages to enable failures to be better reported
- [PN5\_60904](./../pn5_60904/README.md) - Spooler corruption on shutdown
- [PN5\_60907](./../pn5_60907/README.md) - **CREATE-FILE TYPE=JBC** needs to create a dictionary for the source code
- [PN5\_60908](./../pn5_60908/README.md) - Enhance the **DECATALOG** command to delete the intermediate object code that gets generated when a program is compiled
- [PN5\_60909](./../pn5_60909/README.md) - Change how admin privileges are checked in Windows
- [PN5\_60910](./../pn5_60910/README.md) - Add **jDLS** status to **jdiag** output when using **-s** or **-v** option (show services)
- [PN5\_60911](./../pn5_60911/README.md) - Prevent a program aborting while doing a SELECT through a Dynamic File
- [PN5\_60913](./../pn5_60913/README.md) - Remove the restriction which prevents 2 or more copies of jlogdup restoring to the same machine simultaneously
- [PN5\_60914](./../pn5_60914/README.md) - **GET-LIST** in a Proc produced incorrect results in D3 emulation
- [PN5\_60915](./../pn5_60915/README.md) - Transaction Journaling: Prevent a segmentation violation when one of the log sets could not be accessed
- [PN5\_60916](./../pn5_60916/README.md) - Optimize select-list output when the list contains a large number of multi-values (&gt; 100,000)
- [PN5\_60917](./../pn5_60917/README.md) - Spooler: **SP-CREATE Fnn** creates form queues with the wrong queue number
- [PN5\_60919](./../pn5_60919/README.md) - Licensing: Multi-session licenses limited to 255 sessions and up to 255 licenses per session

Back to [Release Notes](./../../releasenotes/../README.md)

<PageFooter />
