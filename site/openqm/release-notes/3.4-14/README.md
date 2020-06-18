# QM 3.4-14 Release Notes

<PageHeader />
Release Date: 12 Mar 2019

* The SP.ASSIGN command has been extended to allow inclusion of SETPTR options.

* Use of @RECORD as the final display clause element in a REFORMAT command appends the entire record with no conversion or formatting applied.

* A dictionary I-type expression can now refer to a field by field number using a name such as "F4" for field 4.

* The QMBasic INPUT statement (but not INPUT @) now has a RAW option that causes it to read a given number of characters with no special interpretation of newline or backspace.

* The QMBasic GETNLS() and SETNLS operations have been extended to allow programmatic control of European date format.

* The QMBasic debugger can now expand non-printing characters when displaying string variables. This is controlled by the "^" command in the same way as its equivalent in the ED editor.

* The default value of the SORTMEM configuration parameter has been increased to 4096 (4Mb) for improved performance. This change affects new QM installations only. The parameter may be modified on existing installations by editing the qmconfig file.

* Setting the USERPOOL configuration parameter to zero changes the way in which the user number is allocated when a user logs in. The default behaviour of QM is to allocate user numbers in a rotating manner. With USERPOOL set to zero, the lowest available user number is assigned.
<PageFooter />
