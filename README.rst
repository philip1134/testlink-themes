===============
TestLink Themes
===============

testlink supports customized themes, we built this project to provide themes
to make testlink display in different style.

``master`` branch supports the latest testlink release, currently is
`TestLink 1.9.20 Raijin <https://github.com/TestLinkOpenSourceTRMS/testlink-code>`__.
we will build different branches to support testlink releases.

Usage
-----

download code
~~~~~~~~~~~~~

download the code of this project, copy ``themes/*`` to ``testlink/gui/themes``.
then ``themes`` folder looks like:

.. code:: text

    testlink
        |- gui
            |- themes
                |- default
                |- grayskin
                |- ...

modify config
~~~~~~~~~~~~~

modify testlink config file ``config.inc.php`` to set theme dir, for example,
we say ``grayskin``:

.. code:: php

    /* almostly line 98 */
    /** GUI themes (base for CSS and images)- modify if you create own one */
    $tlCfg->theme_dir = 'gui/themes/grayskin/';

modify frame.css
~~~~~~~~~~~~~~~~

as `pr209 <https://github.com/TestLinkOpenSourceTRMS/testlink-code/pull/209>`__,
the ``<link>`` to frame.css is hard coded in testlink code, and it links to
``default/css/frame.css``, so we copy ``grayskin/css/frame.css`` to overwrite
``default/css/frame.css``.
