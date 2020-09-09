Using code in .rst files with code-block and literalinclude directives
***********************************************************************
************************
Code Blocks
************************

References: 
------------------------------------------------------------------------------------------------

| https://www.sphinx-doc.org/en/1.5/markup/code.html
| https://bashtage.github.io/sphinx-material/rst-cheatsheet/rst-cheatsheet.html
| 
| We can use code blocks with the .. code-block:: command.
| You will need an empty space, and the code inside will need to be further indented by 3 spaces


.. code-block::

   code-block:: sql

      select * from mytable
      where txn_dt > trunc(sysdate-10)


Typing some code using code-highlight and code-block
-----------------------------------------------------

.. code-block::

   .. code-highlight:: sql
   .. code-block:: sql

      select * from mytable
      where rownum < 5


Take some code from example files with literalinclude and myfilename.ext
------------------------------------------------------------------------
We can use the literalinclude directive to display code as is from a file in a code block. Good for displaying example code. To do so we use:

.. code-block::

   .. literalinclude:: current_portfolio.py
   :language: python
   :linenos:

Which renders as:

.. literalinclude:: current_portfolio.py
   :language: python
   :linenos:




    