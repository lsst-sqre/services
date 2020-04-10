######################
LSST Service Directory
######################

This Sphinx site is an index of services deployed by the Rubin Observatory's SQuaRE team.
View it at https://services.lsst.io.

Contributing
============

1. Create a virtual environment (if you haven't already):

   .. code-block:: bash

      python3 -m venv .venv
      source .venv/bin/activate

   **Tip:** activate this virtual environment in another shell by re-running the ``source`` command.

2. Install dependencies:

   .. code-block:: bash

      python -m pip install --upgrade pip
      python -m pip install -r requirements.txt

3. Build the site:

   .. code-block:: bash

      make html

   Open ``_build/html/index.html`` in a browser to review it.

4. To completely clear the build:

   .. code-block:: bash

      make clean

5. To check links:

   .. code-block:: bash

      make linkcheck

   If some links are behind a login, you might need to ignore them.
   Look at the ``linkcheck_ignore`` variable in ``conf.py`` for examples of how to do this.

Deployment
==========

Whenever you push a GitHub, the site is built for the corresponding branch.
Find your build at https://services.lsst.io/v.

The ``master`` branch is always published as https://services.lsst.io.
