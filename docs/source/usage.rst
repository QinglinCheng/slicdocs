============================
 Using the slicdocs Theme
============================

Guidelines
==========

Prior to using this theme, ensure your project can use the Slic
brand by referring to the brand guidelines at
http://www.slic.org/brand. In particular, if the project is not
under Slic governance as an "official" project, it should not use
this theme.

If your documentation is not being published to an slic.org site,
that may be a signal that you should not use this theme.

Sphinx Configuration
====================

To use the theme, add ``'slicdocs'`` to the ``extensions`` list in
the ``conf.py`` file in your Sphinx project.

Incubating Projects
===================

If you are an incubating project, set::

  html_theme_options = {'incubating': True}

in your conf.py as well, to enable the Incubation theme.

Linking to a Source Repository
==============================

``slicdocs`` defines a configuration option ``docs_cgit_link``
which should be the URL to the git repository browser for the project
being documented. The default is a guess, and will be right for a lot
of projects, but to ensure that it is correct in all situations it is
best to set the value in conf.py::

  docs_cgit_link = 'http://git.slic.org/cgit/slic/slicdocs'

Showing Older Versions of Documentation
=======================================

``slicdocs`` can automatically add links for previous versions of your
project's documentation to the sidebar. If this feature is enabled links
will be generated for each git tag. To enable this behavior, set::

  html_theme_options = {'show_other_versions': True}

in your conf.py.
