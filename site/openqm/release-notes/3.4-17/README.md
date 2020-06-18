# QM 3.4-17 Release Notes

<PageHeader />
Release Date: 8 Nov 2019

* Dictionary I-type item expressions can now use the syntax where a value is followed by a format string with no intervening operator.

* The SAVE.LIST and GET.LIST commands now support use of a multifile.

* QMBasic class modules may now include initialisation values for private and public variables.

* The QMBasic MERGELIST() function now has an additive mode key value to specify that the supplied lists are not in sorted order. This does not affect the MERGE.LIST command.

* Two new keys for the QMBasic SYSTEM() function have been added. Key 1081 returns the current time in milliseconds from 1 January 1970 UTC. Key 1082 returns the time of day as milliseconds since midnight in the user's time zone.

* The !MULTISORT() subroutine provides a way to sort a set of related field mark delimited lists.

* The user written subroutine called by the WEBSVC command now has an optional new argument to pass additional data about the connection.

* Process dump files now include the operating system environment variables.

<PageFooter />
