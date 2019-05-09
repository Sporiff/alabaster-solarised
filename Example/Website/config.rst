=============
Configuration
=============

To get your site up and running with
Sphinx solarized dark, you will need to
do the following.

Setting up Dependencies
-----------------------

Check the :doc:`dependencies  list <deps>`
for the necessary software. Be sure to use
the same version of Python to install each
one.

Setting up Sphinx
-----------------

To initialise your sphinx site, run ``sphinx-quickstart``
and enter the necessary information. This will generate the
necessary files and folders to build and serve your Sphinx site.

If you are using `ablog <http://ablog.readthedocs.io/>`_, run the
`ablog start` command to get the necessary files and folders.

Create a folder called ``_static`` and another folder within
it called ``css``. Place the ``custom.css`` file from the
`repository <https://gitlab.com/sporiff/alabaster-solarized-dark>`_ in
here.

Editing Configuration
---------------------

In order to use the custom CSS and the `pygments-solarized <https://pypi.org/project/pygments-solarized/>`_
linter, we will need to enter the following values in the ``conf.py`` file.

.. code-block:: python

   # Tell the config file to look for a stylesheet in the css folder

   def setup(app):
    app.add_stylesheet('css/custom.css')

   # Tell Pygments to lex using the solarized dark theme

   pygments_style = 'solarized_dark'

   # Make sure your static path is set

   html_static_path = ['_static']

Build the site
--------------

Depending on whether you used Sphinx or Ablog, run ``make html`` or
``ablog build`` respectively. The files should then be built and stored
in the location specified during setup. Open up the ``index.html`` file
to see your site.
