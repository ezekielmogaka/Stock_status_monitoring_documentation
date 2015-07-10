OVERVIEW
============================


The purpose of this project is to establish an hierarchy of the drugs supply chain
that is not captured in DHIS2 for purposes of analysis and report generation.

As things stand, the Kenya instance of DHIS2 only establishes a hierarchy based on 
the countries administrative units which while important, does not capture the
supply chain hierarchy.

The drug supply hierarchy needs to place facilities in their correct order clearly
showing the reporting chain ie what facilities report to what and what facilities
are children so to speak of what facilities.


Facility types
----------------

Four types of facilities used of drugs supply exist:
		#. CENTRAL STORES
		#. CENTRAL STORE DISPENSING POINTS
		#. SATELLITE STORES
		#. STAND ALONE SITES


The reporting hierachy
----------------------
*Central Stores* are at the top and own (in the reporting hierarchy) the central store
dispensing points and the satellite stores.

Central store dispensing points are central points that act as dispensing points 
which means in essence, it is the same facility but acts as both a central store and
a dispensing point.

Satellite stores are facilities that report to the central stores.

Stand alone sites as the name suggests do not have any affiliation in the reporting
hierarchy.

Existing facilities (Level 4) are used as stores for the purpose of drug dispensing.
These facilities are captures in DHIS2 as Level 4 Organization Units and thus no
hierarchy exists between them.

The purpose of this project is to establish that hierarchy.




.. We recommend that you use `Vagrant`_ and `Virtualbox`_ to create a test
.. server for yourself.

.. .. _Vagrant: https://www.vagrantup.com/
.. .. _Virtualbox: https://www.virtualbox.org/
.. .. _Ansible: https://docs.ansible.org

.. If you are an expert Vagrant user, you can substitute Virtualbox with VMWare
.. Desktop / Player, HyperV etc. You'll have an easier time if you are on a
.. ``_nix`` e.g Ubuntu or OS X.


.. Deployment Assumptions
.. -----------------------
.. The deployment scripts will fail unless the following are true:

..   * you are on a vagrant supported OS ( so far Ubuntu 14.04LTS has been tested )
..   * you have run ``ssh-keygen`` and have a public key at ``$HOME/.ssh/id_rsa.pub``

.. Vagrant
.. ----------
.. Before installation, you will need to have the `vagrant-env <https://github.com/gosuri/vagrant-env>`_  plugin.
.. The installation is as simple as running

.. ::

..     vagrant plugin install vagrant-env


.. `Ansible`_ is used to provision the vagrant box. An understanding of ansible is recommended though not required.


.. Installation
.. -----------------

.. 1. Ensure vagrant is installed

.. 2. Create a python virtual environment and activate the created virtual environment.

.. 3. Install ``ansible`` in the virtual environment.

.. 4. Set the following environment variables:

..     - ``DATABASE_NAME`` the name of the database to user
..     - ``DATABASE_USER`` the database user to use
..     - ``DATABASE_PASSWORD`` the database password to use

.. 5. Run ``vagrant up``. It shall download and setup everything in the virtual machine.

.. 6. The system is ready to use

.. toctree::
    :maxdepth: 2
