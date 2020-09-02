Section Header
================================

Subsection Header
--------------------------------

- A bullet list item
- Second item

  - A sub item

- Spacing between items separates list items

* Different bullet symbols create separate lists

- Third item

1) An enumerated list item

2) Second item

   a) Sub item that goes on at length and thus needs
      to be wrapped. Note the indentation that must
      match the beginning of the text, not the 
      enumerator.

      i) List items can even include

         paragraph breaks.

3) Third item

#) Another enumerated list item

#) Second item



A sentence with links to `Wikipedia`_ and the `Linux kernel archive`_.

.. _Wikipedia: https://www.wikipedia.org/
.. _Linux kernel archive: https://www.kernel.org/


Another sentence with an `anonymous link to the Python website`__.

__ https://www.python.org/


::

  some literal text

This may also be used inline at the end of a paragraph, like so::

  some more literal text

.. code:: python

   print("A literal block directive explicitly marked as python code")


SPHINX reStructuredText Primer
--------------------------------

- `documentation link`__

__ https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html

- one asterisk: *text* for emphasis (italics),

- two asterisks: **text** for strong emphasis (boldface), and

- backquotes: ``text`` for code samples.

    it may not be nested,

    content may not start or end with whitespace: * text* is wrong,

    it must be separated from surrounding text by non-word characters. Use a backslash escaped space to work around that: thisis\ *one*\ word.

* This is a bulleted list.
* It has two items, the second
  item uses two lines.

1. This is a numbered list.
2. It has two items too.

#. This is a numbered list.
#. It has two items too.

* this is
* a list

  * with a nested list
  * and some subitems

* and here the parent list continues


This is a normal text paragraph. The next paragraph is a code sample::

   It is not processed in any way, except
   that the indentation is removed.

   It can span multiple lines.

This is a normal text paragraph again.


+------------------------+------------+----------+----------+
| Header row, column 1   | Header 2   | Header 3 | Header 4 |
| (header rows optional) |            |          |          |
+========================+============+==========+==========+
| body row 1, column 1   | column 2   | column 3 | column 4 |
+------------------------+------------+----------+----------+
| body row 2             | ...        | ...      |          |
+------------------------+------------+----------+----------+


=====  =====  =======
A      B      A and B
=====  =====  =======
False  False  False
True   False  False
False  True   False
True   True   True
=====  =====  =======

This is a paragraph that contains `a link`_.

.. _a link: https://domain.invalid/

::

    def my_function(my_arg, my_other_arg):
        """A function just for me.

        :param my_arg: The first of my arguments.
        :param my_other_arg: The second of my arguments.

        :returns: A message (just for me, of course).
        """

For footnotes (ref), use [#name]_ to mark the footnote location, and add the
footnote body at the bottom of the document after a “Footnotes” rubric
heading, like so::


Lorem ipsum [#f1]_ dolor sit amet ... [#f2]_

.. rubric:: Footnotes

.. [#f1] Text of the first footnote.
.. [#f2] Text of the second footnote.

.. This is a comment.