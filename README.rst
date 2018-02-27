======
Pipenv
======
Love it, hate it
----------------

*The “officially recommended” Python packaging tool*

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

Scaling
-------

To get scaling to show as 1:1 when the browser window matches the configured
size edit ``hovercraft/templates/simple/template.xsl`` to include
``data-width`` and ``data-height`` similarly to ``data-perspective`` which was
implemented in https://github.com/regebro/hovercraft/pull/75

.. code::

      <div id="impress">
        <xsl:if test="@data-perspective">
          <xsl:attribute name="data-perspective">
            <xsl:value-of select="@data-perspective" />
          </xsl:attribute>
        </xsl:if>
        <xsl:if test="@data-width">
          <xsl:attribute name="data-width">
            <xsl:value-of select="@data-width" />
          </xsl:attribute>
        </xsl:if>
        <xsl:if test="@data-height">
          <xsl:attribute name="data-height">
            <xsl:value-of select="@data-height" />
          </xsl:attribute>
        </xsl:if>

.. vim: ft=rst
