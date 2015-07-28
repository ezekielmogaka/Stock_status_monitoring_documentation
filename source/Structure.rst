Project structure
======================
The malaria stock status monitoring tool contains three parts: 

	#. Assets
	#. Client
	#. Database
	#. System

Each part is crucial for this project.

Assets
------
These are the resources needed in this project. 

It contains:

	- CSS
	- Bootstrap
	- PHP - CodeIgniter framework
	- JavaScript 

Client
------
- This is the presentation and user interface logic. 

- It contains scripts that will display on the browser. The client side is linked to the server side so that the user can make use of the server side logic.

Database
---------
This is the database logic. It contains scripts for database authentication and connection creation as well as those for inserting, fetching and updating items on the database.




System
-------

- This is the system environment variables. It contains parameters that need to be set for the system to run once deployed.

- They include the database authentication and connection creation.

- Edit the config (config.php) file to reflect your local environment.

- The project's landing page is at:  http://msh.urandu.com/. It is the login page.



.. .. note::

..     All the assets listed above have to be available for the system to work


.. toctree::
    :maxdepth: 2
