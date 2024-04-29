Template for the Read the Docs tutorial
=======================================

This GitHub template includes fictional Python library
with some basic Sphinx docs.

Read the tutorial here:

https://docs.readthedocs.io/en/stable/tutorial/

Build Locally
=============

.. code-block:: console

    # prepare venv
    conda activate ./env
    python -m pip install --upgrade --no-cache-dir pip setuptools
    python -m pip install --upgrade --no-cache-dir sphinx readthedocs-sphinx-ext
    python -m pip install --exists-action=w --no-cache-dir -r docs/requirements.txt

    # make docs
    cd docs
    make html
