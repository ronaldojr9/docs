# QM 3.4-18 Release Notes

<PageHeader />
Release Date: 14 Feb 2020

* The CLOSE.ECI command terminates all External Call Interface child processes started by the process in which the command is executed.

* For compatibility with other systems, QM now supports the DECATALOG command to delete a local catalogue entry and its object code.

* The LIST.READU and PSTAT commands now show the time at which a blocked process started waiting for a lock. This information is also returned by the QMBasic GETLOCKS() function.

* The SED editor now has split up and split down functions to allow movement of the split point in a split window.

* An optional $VLIST control record has been added to dictionaries and the VOC to override the default determination of the name column width.

* A vertical mode query processor report now makes it easier to distinguish between multivalued data and a long line that has wrapped. In the latter case, the colon before the data is omitted on all but the first line.

* A new $MODE setting, TIME.MS, has been added to cause TIME() and SYSTEM(12) to return the time to millisecond precision as a floating point value.

* A new $MODE setting, STRICT.EQUATE, has been added to show a warning if the token name set by EQUATE or $DEFINE is also a statement name, function name or reserved word.

* The QMBasic GET statement reads data from a device, typically a serial port.

* The QMBasic INPUTIF statement returns any data in the type-ahead buffer or in the DATA queue.

* For improved compatibility, the QMBasic STATUS statement now returns field 27 as the file pathname.

* The QMBasic SYSTEM() function key 35 (SYS$USERS) returns the current number of users.

* The QMBasic SYSTEM() function key 1083 (SYS$DEADLOCK) returns information about the most recent deadlock for use where an application catches the deadlock exception.

* Several tools to assist in migrating to QM and procedure documentation have been added.

<PageFooter />
