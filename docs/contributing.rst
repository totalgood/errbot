Contributing
============

If you would like to contribute to the project, please do not hesitate to get
involved! Here you can find how best to get started.

Contributing to Errbot itself
-----------------------------

Clone Errbot
~~~~~~~~~~~~

All development on Errbot happens on GitHub_. If you'd like to get involved, just
fork_ the repository and make changes in your own repo. When you are satisfied
with your changes, just open a `pull request`_ with us and we'll get it reviewed
as soon as we can! Depending on our thoughts, we might decide to merge it in
right away, or we may ask you to change certain parts before we will accept the
change.

Run Errbot from source
^^^^^^^^^^^^^^^^^^^^^^

Clone you github fork repo locally and install errbot in development mode from the root of the repo with::

    pip install -e .

From there, anytime you execute `errbot` it will run from the checked out version of Errbot with all your local
changes taken into account.

Preparing your pull request
^^^^^^^^^^^^^^^^^^^^^^^^^^^

In order to make the process easy for everyone involved, please follow
these guidelines as you open a pull request.

* Make your changes on a separate branch_, preferably giving it a descriptive name.
* Split your work up into smaller commits if possible, while making sure each commit
  can still function on its own. Do not commit work-in-progress code - commit it
  once it's working.
* Run tox before opening your pull request, and make sure all tests pass.
  You can install tox with :command:`pip install tox`
* If you can, please add tests for your code. We know large parts of our codebase
  are missing tests, so we won't reject your code if it lacks tests, though.

Contributing documentation & making changes to the website
----------------------------------------------------------

`errbot.io <http://www.errbot.io/>`_ is created using Sphinx_, which also doubles
as a generator for our (API) documentation. The code for it is in the same repository
as Errbot itself, inside the docs_ folder. To make changes to the documentation or the
website, you can build the HTML locally as follows::

    # Change directory into the docs folder
    cd docs/
    # Install the required extra dependencies
    pip install -r requirements.txt
    # Generate the static HTML
    make html
    # Then, open the generated _build/html/index.html in a browser

To submit your changes back to us, please make your change in a separate branch as
described in the previous section, then open a pull request with us.

.. note::
    You must do this with Python 3, Python 2 is unsupported.

Issues and feature requests
===========================

Please report issues or feature requests on the `issue tracker`_ on GitHub.

When reporting issues, please be as specific as possible. Include things such as
your Python version, platform, debug logs, and a description of what is happening.
If you can tell us how to reproduce the issue ourselves, this makes it a lot
easier for us to figure out what is going on, as well.

Getting help
============

The best place to get help if you get stuck with anything is to ask for advice
on our Gitter_ chat room. If nobody is around to help you, opening an issue on
the `issue tracker`_ is your next best option.

If you have a code-related question concerning (plugin) development it's best
to ask your question on Stack Overflow, `tagged errbot
<http://stackoverflow.com/questions/tagged/errbot>`_.

.. _GitHub: https://github.com/errbotio/errbot
.. _fork: https://github.com/errbotio/errbot/fork
.. _`pull request`: https://help.github.com/articles/using-pull-requests
.. _branch: http://git-scm.com/book/en/Git-Branching
.. _Sphinx: http://sphinx-doc.org/
.. _docs: https://github.com/errbotio/errbot/tree/master/docs/
.. _repos.py: https://github.com/errbotio/errbot/blob/master/errbot/repos.py
.. _`issue tracker`: https://github.com/errbotio/errbot/issues/
.. _Gitter: https://gitter.im/errbotio/errbot
