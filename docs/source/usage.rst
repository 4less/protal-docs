Usage
=====

.. _installation:

Installation
------------

Protal is written in C++ and can be installed from multiple sources.

bioconda
^^^^^^^^

.. code-block:: console

   (conda_env) $ conda install protal

Prebuilt binaries
^^^^^^^^^^^^^^^^^

Go to github.

.. code-block:: console

   $ wget 

Build from sources
^^^^^^^^^^^^^^^^^^

Go to github.

.. code-block:: console

   $ wget 

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

