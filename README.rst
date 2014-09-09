yasfb
=====

This Sphinx extension is derived Fergus Doyle's `sphinxfeed
<https://github.com/junkafarian>`_ which is in turn derived from Dan
Mackinlay's `sphinxcontrib.feed
<http://bitbucket.org/birkenfeld/sphinx-contrib/src/tip/feed/>`_
package.

Usage
-----

#. Install ``yasfb`` using ``easy_install`` / ``pip`` /
   ``python setup.py install``

#. Add ``yasfb`` to the list of extensions in your ``conf.py``::

       extensions = [..., 'yasfb']

#. Customise the necessary configuration options to correctly generate the
   feed::

       feed_base_url = 'http://YOUR_HOST_URL'
       feed_author = 'YOUR NAME'

Publishing Dates
----------------

Publish dates for feed entries come from either reST metadata embedded
in the file, or the last git commit date for a file.

