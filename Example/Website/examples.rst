========
Examples
========

Notes and Warnings
------------------

.. note::

   This is a note. It matches the background
   but has a slightly clearer colour scheme

.. warning::

   Warnings make use of the solarized light
   theme to make them stand out

Code
----

Python
^^^^^^

.. code-block:: Python

   import os
   import sys
   import alabaster

   def setup(app):
       app.add_stylesheet('css/custom.css')

   project = 'Alabaster Solarized Dark'
   copyright = '2019, Ciarán Ainsworth'
   author = 'Ciarán Ainsworth'

   release = '1.0.0'

   extensions = [
       'alabaster'
   ]

   pygments_style = 'solarized_dark'

   html_theme = 'alabaster'

   html_static_path = ['_static']

CSS
^^^

.. code-block:: css

   body {
       font-family: Georgia, serif;
       font-size: 17px;
       color: #839496;
       background-color: #002b36;
   }

   div.body {
       background-color: #002b36;
       color: #839496;
   }

   tt,
   code {
       color: #d30102;
   }

Headers
-------

H2
--

H3
^^

H4
**
