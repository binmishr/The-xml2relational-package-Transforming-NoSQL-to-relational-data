# The-xml2relational-package-Transforming-NoSQL-to-relational-data

The details of the codeset and plots are included in the attached Adobe Acrobat reader (.pdf) file in this repository. 
You need to download the same to view the contents. There are referrals to other contents in BLUE colour also to follow.

Introduction
===============

In contrast to many other programming languages, R has no real native switch-case statement. It does provide the primitive switch() function; but switch() is actually made to select elements from a list based on their name or index position. It cannot (at least not without awkward workarounds) be used to build conditions with more complex comparison values. Also, when fed with a numeric expression, it interprets the expression as an index and selects the element from the list at this index position. This is not useful when you want to test an expression against another numeric expression/value.

It would be good to have an efficient way of testing multiple, similar conditions, including conditions that are more complex in their comparison values or result in numeric values. At the same time nested if-else constructs should be avoided because they make the code less clear and readable.

The switchcase package provides a solution by offering a true switch-case construct for R. It is encapsulated in the package’s main function, switchCase().

switchCase() allows to define multiple ‘case’ branches (alternatives) that consist of a condition and a code block that is executed if the condition is fulfilled. Also, it can be specified if the switch-case construct shall be left after one alternative code block has been executed, or if the other (following) conditions shall be tested, as well. This ‘break’ behavior can be defined on the level of the whole switch-case construct or on the level of each individual alternative, with the alternative’s ‘break’ behavior setting overruling the construct-level option. Also, an alternative branch of a switch-case construct can return a value (which is then the return value of the switchCase() function).

Installing switchcase
======================

Before using switchCase() we need to install and load the package:

install.packages("switchcase", dependencies = TRUE)

library(switchcase)
