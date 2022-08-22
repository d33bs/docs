Development
===========

Development for Cytomining Docs takes place using `reStructuredText (RST) <https://www.writethedocs.org/guide/writing/reStructuredText/>`_ implemented by `Python <https://www.python.org/>`_ environments managed by `Poetry <https://python-poetry.org/>`_.
RST documents are transformed into docsite content using `Sphinx <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_.

Getting Started
---------------

Local development may be enabled using roughly the following steps.

1. `Install Python <https://www.python.org/downloads/>`_
2. `Install Poetry <https://python-poetry.org/docs/#installation>`_
3. `Install Poetry Environment <https://python-poetry.org/docs/basic-usage/#installing-dependencies>`_
4. Use the IDE of your choice to add or edit related content.

Lint
----

Linting the Sphinx RST files is performed automatically using Github Actions `Github Action <https://github.com/features/actions>`_.
You can also lint the documentation locally using the command ``poetry run sphinx-lint``.

Build
-----

RST documents may be converted into HTML content using Sphinx.
`Reference this page for build implementation details <https://www.sphinx-doc.org/en/master/usage/quickstart.html#running-the-build>`_.

Deploy
------

Deployment of the HTML content referenced for the build is used as part of `Github Pages <https://pages.github.com/>`_ and a related  to assist with automation.
