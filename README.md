# ASN1BER
ASN1BER is a package that supports the Abstract Syntax Notation One and Basic Encoding Rules, as defined by ISO 8824 and ISO 8825. These
standards provide specifications for representing data abstractly (like
a programming language) and concretely (i.e., machine-independent
bit-level encoding rules).  ASN.1 and BER are used in a variety of
communications environments, including SNA, OSI and TCP/IP.

The ASN1BER package contains these components:

1. The ASN1 program compiles the abstract syntax.  All ASN.1 constructs
(except macros) are supported.  Support for Script and Bookmaster source
files is included.  The compiled output is a machine-independent
representation of the abstract syntax that must be translated by a
machine-dependent version of TBLXLATE.

2. The TBLXLATE translates the machine-dependent output of ASN1 into
several forms which are specific to the application execution
environment.

3. The runtime encode/decode routines are link-edited with the
application program and work with the output of the TBLXLATE
program to build and parse BER data.  One distinguishing feature of
these routines is that they allow dynamic loading and unloading of
ASN.1 modules.

4. The SORTRES program is used as an aid in porting the ASN1 compiler to
other host environments.

5. The ENCDEC program is a sample program that illustrates use of many
of the runtime libraries and may be used to "play" with abstract syntax.

6. Source code for all of the above.

7. Documentation, including a lengthy description of the ASN.1 syntax.

The ASN1BER package has been successfully ported to the OS/2, DOS,
AIX/6000, and VM/CMS systems.
