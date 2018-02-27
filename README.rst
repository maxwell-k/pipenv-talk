======
Pipenv
======
Love it, hate it
----------------

*The “officially recommended” Python packaging tool*

`26 February 2018 PyBelfast`_

Install packages:

.. code:: sh

    npm install -g reload
    pip install --global hovercraft # see Scaling below

Build the presentation with:

.. code:: sh

    hovercraft talk.txt public

In another terminal:

.. code:: sh

    cd public && reload

Then browse to http://localhost:8080/

The ``div#impress`` is the root element for the hovercraft presentation.
When the browser is full screen, this will be styled with ``scale(1)`` if the
browser is not full screen this will show a value less than 1.

.. _26 February 2018 PyBelfast:
    https://www.meetup.com/PyBelfast/events/247837520/

.. vim: ft=rst foldmethod=manual
