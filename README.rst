sphinxfeed
==========

This Sphinx extension is derived from Dan Mackinlay's `sphinxcontrib.feed
<http://bitbucket.org/birkenfeld/sphinx-contrib/src/tip/feed/>`_ package.

This project has received significant contributions from
`yasfb <https://github.com/dhellmann/yasfb>`_ by Doug Hellman.

It relies on the `feedformatter <http://code.google.com/p/feedformatter/>`_
package instead of Django utils to generate the feed.

Usage
-----

#. Install ``sphinxfeed`` using ``easy_install`` / ``pip`` /
   ``python setup.py install``

#. Add ``sphinxfeed`` to the list of extensions in your ``conf.py``::

       extensions = [..., 'sphinxfeed']

#. Customise the necessary configuration options to correctly generate the
   feed::

       feed_base_url = 'http://YOUR_HOST_URL'
       feed_author = 'YOUR NAME'

Publishing Dates
----------------

Publish dates for feed entries come from either reST metadata embedded
in the file, or the last git commit date for a file.
