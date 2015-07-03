=================
Code Requirements
=================

To make sure that your code can be integrated smoothly into the existing codebase, there are some requirements which your code should meet:

Code Style
==========

All Monospark projects follow the `Google Java Style Guidelines <https://google-styleguide.googlecode.com/svn/trunk/javaguide.html>`_.
Furthermore, there are some custom modifications to these guidelines, which are listed here:

Column Width
------------

The column width, which represents the maximum amount of characters per line, is:

* 120 for code and comments, because it's makes diffs easier to read.
* 80 for Javadocs, because the Javadoc text gets wrapped at 80 characters and that would mess up the formatting.

Indentation
-----------

* For Indentation, 4 spaces are used. Do not use tabs or any other amount of spaces.
* Lines, which were wrapped because they were exceeding the 120 character column width, are indented with 6 spaces instead of 4.

Line Endings
------------

For line endings, the Unix newline character Line Feed (LF, \\n, U+000A) is used.

.. important::
   Since Windows uses CRLF as a newline character, Windows users must configure Git to automatically convert CRLF line endings to LF.
   This is done by setting the value "core.autocrlf" in your Git System Settings to "true" (``git config --global core.autocrlf true``).

Blank Lines
-----------

* Place a blank line before the first member of a class, interface, or enum.
* Add a blank line to the end of every file, because all lines should be ended with a newline character. 

Code Conventions
================

Usage of New Features
---------------------

All Monospark projects currently target Java 8 for source and compilation.
As a result, you have access to all the new Java Features, so you should use:

* `Optionals <http://docs.oracle.com/javase/8/docs/api/java/util/Optional.html>`_ instead of returning ``null`` (at least in the API, private methods can still return null)
* `Lambda Expressions <https://docs.oracle.com/javase/tutorial/java/javaOO/lambdaexpressions.html>`_ and Functional Programming in the API
* `Streams <http://docs.oracle.com/javase/8/docs/api/java/util/stream/package-summary.html>`_
* `Objects.requireNonNull() <http://docs.oracle.com/javase/7/docs/api/java/util/Objects.html#requireNonNull%28T,%20java.lang.String%29>`_ when checking if arguments are ``null``

Javadocs
--------

Every Javadoc should contain:

* A summary fragment.
* Non-Empty ``@param`` tags for every parameter.
* A non-empty ``@return`` tag with description.
* Non-Empty ``@throws`` tags for every checked exception that can be thrown.

.. hint:: 
   Tips and tricks for writing good Javadocs can be found in the `Javadoc Documentation <http://www.oracle.com/technetwork/java/javase/documentation/index-137868.html>`_

Testing
-------

All Monospark projects employ `JUnit <http://junit.org/>`_ for testing.
Since writing unit tests ensures that newly added features can be easily maintained over time, you should write unit tests for every feature you add to the codebase.
To improve readability, every unit test should follow `Roy Osherove's naming standards for unit tests <http://osherove.com/blog/2005/4/3/naming-standards-for-unit-tests.html>`_ and the AAA (\ **A**\ rrange, \ **A**\ ct, \ **A**\ ssert) pattern.
