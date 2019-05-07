*****************
pgAdmin4 buildout
*****************

Setups and runs pgAdmin4 server. I found that it's quite annoying and hard to get
pgAdmin4 configured and running, so I created a buildout config to automate this
process.

To change running port or version of ``pgAdmin4`` edit following options in ``buildout.cfg`` file:

.. code-block:: ini

    port = 5050
    pgadmin4-version = 4.6

To have it's installed run ``buildout``.
You can install ``buildout`` with ``pip``. 


.. code-block:: bash

    cd pgadmin4-buildout
    pip install zc.buildout
    buildout
    
After installation is done, open  `127.0.0.1:5050 <http://127.0.0.1:5050/>`_.

Tested only in python 3.6 and 3.7.
