===============
TestLink Themes
===============

testlink supports customized themes, we built this project to provide themes
to make testlink display in different style.

this branch supports
`TestLink 1.9.17 Alan Turing <https://github.com/TestLinkOpenSourceTRMS/testlink-code/tree/1.9.17>`__.

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
using ``grayskin`` as:

.. code:: php

    /* almostly line 76 */
    /** GUI themes (base for CSS and images)- modify if you create own one */
    $tlCfg->theme_dir = 'gui/themes/grayskin/';
