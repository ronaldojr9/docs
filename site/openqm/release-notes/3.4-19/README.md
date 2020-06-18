# QM 3.4-19 Release Notes

<PageHeader />
Release Date: 26 May 2020

* The inline prompt construct now allows substitution of a QM configuration parameter using <>.

* The extension introduced at QM 3.4-11 to the mc4 and mc5 terminfo capability definitions to allow selection of the slave printer hsa been reworked to remove the AccuTerm control codes from the terminal definition. This may require changes to user defined terminfo items.

* For improved compatibility with other multivalue systems, QM now supports the CALL conversion code to call a user supplied subroutine.

* The WEBSVC command has been extended to provide a way in which large message body texts can be passed as a file instead of an in-memory string.

* The QMBasic DTX() function can now handle values greater than 2^31.

* The QMBasic FCONTROL() function with action key FC$VALID.ID tests whether the qualifier is a valid record id for the specified file.

* The QMBasic JBUIILD() function has been extended to add an optional mode setting that causes data types that cannot be represented in JSON such as a file variable to be saved as a null item. Previously, a run time error would have occurred.

* The QMBasic REVREMOVE statement extracts elements of a dynamic array in reverse order.

* The QMBasic !CALLHTTP() class module now exposes the HTTP status code via the public HTTP.STATUS variable.

* The QMBasic !PSTAT() subroutine allows an application to request data for a specified QM process similar to that reported by the PSTAT command.

* A new configuration parameter, USPLIT, selects a user number allocation strategy in which interactive users are allocated the lowest available user number and all other process types are allocated the highest available user number.
<PageFooter />
