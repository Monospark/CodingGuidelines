================
Code Conventions
================

To make sure that your code can be integrated smoothly into the existing codebase, you should be following these guidelines:

* Use Java 8 for compilation (Usage of the new Java 8 Features is welcome)
* Follow the `Sun/Oracle coding standards: <http://www.oracle.com/technetwork/java/codeconvtoc-136057.html>`_
* Use 4 spaces for indentation and no tabs
* Limit your columns to 120 characters 
* Use LF line endings only (Set the value "core.autocrlf" in your Git System Settings to "true")
* Add a new line to end of every file
* Write comments if necessary (Recommeneded for complex code)
* Write complete Javadocs (A short description, @param tags, @return tags, and @throws tags are required)
* Write unit tests (All Monospark projects use JUnit and follow `Roy Osherove's naming strategy <http://osherove.com/blog/2005/4/3/naming-standards-for-unit-tests.html>`_)
* Most importantly: Write good, effective and maintainable code