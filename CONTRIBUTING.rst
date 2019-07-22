Guidelines for Contributing
===========================

Individual or groups are very welcome to contribute to pymcmcstat_examples.  There are three main ways of contributing to the pymcmcstat_examples project:

1. Adding useful examples of how to do things with pymcmcstat.
2. Fixing/updating existing examples to provide better clarity.
3. Submitting issues related to bugs or confusion regarding existing examples.

Opening issues
==============

The best way to announce issues is via `Github Issue Tracker <https://github.com/prmiles/pymcmcstat_examples/issues>`_.  Please verify that your issue is not being currently addressed by other issues or pull requests by using the GitHub search tool to look for key words in the project issue tracker.

Contributing code via pull requests
===================================

The recommended workflow for contributing to pymcmcstat_examples is to fork the `GitHub repository <https://github.com/prmiles/pymcmcstat_examples>`_, clone it to your local machine, and develop on a feature branch.

Steps:
------

1. Fork the `project repository <https://github.com/prmiles/pymcmcstat_examples>`_ by clicking on the 'Fork' button near the top right of the main repository page. This creates a copy of the code under your GitHub user account.

2. Clone your fork of the pymcmcstat repo from your GitHub account to your local disk, and add the base repository as a remote:

::

   $ git clone git@github.com:<your GitHub handle>/pymcmcstat_examples.git
   $ cd pymcmcstat_examples
   $ git remote add upstream git@github.com:prmiles/pymcmcstat_examples.git

3. Create a ``feature`` branch to hold your development changes:

::

   $ git checkout -b my-feature

Always use a ``feature`` branch. It's good practice to never routinely work on the ``master`` branch of any repository.

4. Project requirements are in ``requirements.txt``. It is recommended that you use some type of `virtual environment <https://docs.python.org/3/tutorial/venv.html>`_ for your code development.  To install the required packages run:

::

   $ pip install -r requirements.txt

5. Develop the feature on your feature branch. Add changed files using ``git add`` and then ``git commit`` files:

::

   $ git add modified_files
   $ git commit
   
to record your changes locally. After committing, it is a good idea to sync with the base repository in case there have been any changes:

::

   $ git fetch upstream
   $ git rebase upstream/master

Then push the changes to your GitHub account with:

::

   $ git push -u origin my-feature

6. Go to the GitHub web page of your fork of the pymcmcstat_examples repo. Click the 'Pull request' button to send your changes to the project's maintainers for review. This will send an email to the committers.

Pull request checklist
----------------------

We recommended that your contribution complies with the following guidelines before you submit a pull request:

* If your pull request addresses an issue, please use the pull request title to describe the issue and mention the issue number in the pull request description. This will make sure a link back to the original issue is created.

* The tutorial should contain adequate annotation for a user to understand the basic workflow, and it should reference articles as necessary if the tutorial relates to a specific research project.
