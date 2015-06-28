============
Guidelines
============

First of all thank you for showing interest in contributing to a Monospark project!

Code Requirements
=================

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

Making the Changes
==================

1. Fork the project you want to contribute to
2. Create a new branch on your fork (The name of the branch should reflect what you are looking to make)
3. Commit your changes to that branch. Here are some `tips for your commit messages <http://who-t.blogspot.de/2009/12/on-commit-messages.html>`_
4. Submit a pull request to the relevant repository. Before you submit it, you can perform the checklist below:

   * Does your change fit with the goals of the relevant project?
   * Does your code meet the Code Requirements?
   * Are all tests passing?
   * Is your pull request rebased to the latest commit of the target branch? If not, `rebase it <https://help.github.com/articles/about-git-rebase/>`_
