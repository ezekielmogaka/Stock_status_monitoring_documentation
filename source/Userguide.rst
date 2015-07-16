**User guide**
===============

Introduction
------------
MSH/HCSM is a key member of the Malaria drug management subcommittee, which is involved in the stockstatus monitoring 
of Malaria commodities both at the National and County levels.

On a monthly basis, the Malaria Control Unit, drug management committee meets to review the stock status ofmalaria commodities 
in the country, by analyzing data from various sources including:
	#. Facility and County Level Stock Data from DHIS.
	#. National Level Stock Status data from the Supply Chain Agencies (KEMSA).
	#. Pipeline information based on incoming shipments per funding agency.

This data is aggregated and analyzed for the different malaria commodities and a 2 pager report generated that
indicates to management, the months stock status and pipeline monitoring of Malaria commodities. Currently
MCU uses an excel based tool to generate this information. The current requirement is to amend and enhance
the current 2 pager tool to accommodate additional requirements including representation of Central and
county level data for Malaria commodities, and to color code the different pending shipments based on the
timelines for delivery. This request makes the current tool being used to develop the 2 pager report redundant
as it will not meet the requirements of the Malaria control unit and the donor, hence the need to develop a new
tool.

.. _`DHIS2`: https://www.dhis2.org/

Getting started
---------------
Purpose of this project is to create a stock status management tool that analyzes data from various sources including:

#. Facility and County Level Stock Data from DHIS.
#. National Level Stock Status data from the Supply Chain Agencies (KEMSA).
#. Pipeline information based on incoming shipments per funding agency.

System requirements
~~~~~~~~~~~~~~~~~~~
Chrome/Chromium browser is recommended for the application. This is because of the javascript used in the application wil be able to load faster.

Login roles to the stock status management tool are also required inorder to access the application and its functionality.






`Authentication`_ is the process by which clients send login credentials over the HTTP to a web server. The request is 
associated with a specific user, while `authorization`_ determines if the user has permission to perform
the requested operation.

.. _`Authentication`: https://www.dhis2.org/doc/snapshot/en/developer/html/ch01s02.html
.. _`authorization`: https://www.dhis2.org/doc/snapshot/en/developer/html/ch01s02.html


Session Authentication
~~~~~~~~~~~~~~~~~~~~~~~~
Logging in
+++++++++++++
You have to loggin to the Stock management tool to access most of its functionality.
 The payload should be similar to the example below:

.. code-block:: javascript

    {
        "username": "username",
        "password": "password"
    }

.. note::

    A successiful login will lead you to using the application.

Here is the login page:

 	
	.. figure:: images/login.png

After successiful login, the homepage is loaded.

    .. figure:: images/home.png

Logging out
++++++++++++++

.. note::
    A user can logout after using the tool by clicking the logout button located in the header.


A successful logout will bring up a  success message similar to the one below:

.. code-block:: javascript

    {
        "success": "Successfully logged out."
    }



Permissions
-------------
Login roles
~~~~~~~~~~~~~
There are various user roles according to the user who is logged in:

    #. **Normal Users** who can only only read data ie generating and viewing reports. These kind of users have no permissions to change anything in the application.

    #. **The Admin** who has all the permissions in the application. These include:

        - Creation and management of users
        - Updating data that is used to generate reports


Launching the Application
--------------------------

The stock status application is launched as a stand alone application since it is not incorporated in DHIS2. However, the application pulls data from DHIS2.

For the application to be launched, this `link`_  has to be typed in the browser. The link redirects the user to the login page.

.. _`link`: http://msh.urandu.com/new/index.php/


Application Layout
-------------------
Header
~~~~~~~
The header of the application has no menu. It has the message: *Malaria Commodities Stock Monitoring Tool*. It also has the log out icon.


Side bar
~~~~~~~~~
The side bar of the aplication has an array of links. They include the following:

Dashboard
+++++++++++
This link redirects to the homepage of the application.


Manage
+++++++
This link enables the admin to manage the following:

    - Funding agencies
    - Supply chain agencies
    - Commodities
    - Counties
    - Zones
    - Forecasts

Stocks
++++++
This link allows users to view a report on the malaria stock. It includes:

    - Pending shipments
    - Current stock


Reports
+++++++
This link is used to query various reports from the application. The reports include:

    - Central level MOS
    - Forecast data MOS
    - Facility level MOS
    - National level MOS
    - County level NOS
    - Stocks
    - Commodities
    - Agencies

Manage Users
+++++++++++++

Here, the admin can view the list of the users registered in the system. The admin has the permissions of adding new users and updating their details.
    





**User tasks**
---------------



**Setup**
----------

Funding Agency
~~~~~~~~~~~~~~~
This loads the panel for managing the funding agencies. The user clicks a funding agency from the list given for editing or deleting.

    .. figure:: images/fundingAgency.png

After choosing one of the agencies, a user can edit or delete it.
    .. figure:: images/manageAgency.png

A user can also add a funding by clicking the button of adding an agency.

    .. figure:: images/addAgency.png




Supply chain agencies
~~~~~~~~~~~~~~~~~~~~~~
This loads the panel for managing the supply chain agencies. The user clicks a supply chain agency from the list given for editing or deleting.

    .. figure:: images/supplyChainAgency.png

After choosing one of the supply chain agencies, a user can edit or delete it.
    .. figure:: images/addEditSupplyAgency.png

A user can also add a supply chain agency by clicking the button of adding a supply chain agency.

    .. figure:: images/addSupplyChainAgency.png



Commodities
~~~~~~~~~~~~
This loads the panel for managing the individual commodities. The user clicks a commodity from the list given for editing or deleting.

    .. figure:: images/commodity.png

After choosing one of the commodities, a user can edit or delete it.
    .. figure:: images/editCommodity.png

A user can also add a commodity by clicking the button of adding a commodity.

    .. figure:: images/addCommodity.png



Counties
~~~~~~~~~
This loads the panel for viewing and updating counties. The user clicks a specific county from the list given for updating details about it.

    .. figure:: images/counties.png

After choosing one of the counties, a user can edit the zone and/or the comment about it.
    .. figure:: images/updateCounty.png

Static parameters
~~~~~~~~~~~~~~~~~~
This loads the panel for managing the static parameters. The user clicks an item from the list given for editing or deleting.

    .. figure:: images/staticParamter.png

After choosing one of the static parameters, a user can edit or delete it.
    .. figure:: images/editStaticParameter.png

A user can also add a static parameter by clicking the button of adding a static parameter.

    .. figure:: images/addStaticParameter.png


**Transactions**
-----------------

Pending shipments
~~~~~~~~~~~~~~~~~~~
This loads the panel for managing the pending shipments. The user clicks an item from the pending stock list given for editing or deleting.

    .. figure:: images/pendingShipment.png

After choosing one of the pending stock, a user can edit or delete it.
    .. figure:: images/editDeletePendingStock.png

A user can also add a new transaction by clicking the button of adding a new transaction.

    .. figure:: images/addPendingStock.png



    
Confirmed shipments
~~~~~~~~~~~~~~~~~~~~

Current Stock
~~~~~~~~~~~~~~~
This loads the panel for managing the current stock. The user clicks an item from the current stock list given for editing or deleting.

    .. figure:: images/currentStock.png

After choosing one of the current stock commodities, a user can edit or delete it.
    .. figure:: images/editDeleteCurrentStock.png

A user can also add a new record by clicking the button of adding a new record.

    .. figure:: images/addCurrentStock.png


**Reports**
----------
Central level MOS Report(Forecast)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
A report on central level MOS using forecast data. It reports on the following:

    #. Commodity name
    #. Aggregated Adjusted Consumption Totals
    #. Aggregated Stock on Hand Totals 
    #. Central level MOS 

    .. figure:: images/centralLevelMOSforeCast.png




Central level MOS Report(DHIS2)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
It shows a report on the central level MOS from DHIS2. It reports on the following:

    #. Commodity name
    #. Aggregated Adjusted Consumption Totals
    #. Aggregated Stock on Hand Totals 
    #. Central level MOS 

    
    .. figure:: images/centralLevelMOSReport.png


County level MOS Report(DHIS2)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
It generates a report on the county level MOS. It reports on:

    #. Commodity name
    #. Aggregated Adjusted Consumption Totals 
    #. Aggregated Stock on Hand Totals 
    #. County level MOS 

    .. figure:: images/countyLevelMOSReport.png
    



Current/Pending
~~~~~~~~~~~~~~~~~
It shows a report on the current/pending commodities. It reports on the following:

    #. Stock on Hand(SOH)
    #. Total Pending consignments
    #. MOS
    #. Commodity
    #. Individual Agencies & Quantity

    .. figure:: images/current_pendingCommodities.png
    

Total pending commodities
~~~~~~~~~~~~~~~~~~~~~~~~~~
This shows a report on the total pending . It shows the following details:

    #. Commodity
    #. Totals
    

    .. figure:: images/totalPendingStock.png


Individual pending commodities
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
This shows a report on the individual pending stock. It shows the following details:

    #. Commodity
    #. Supporting agency
    #. Quantity
    #. E.T.A Details

    .. figure:: images/pendingStockReport.png



Commodities/Agency
~~~~~~~~~~~~~~~~~~~

This shows a report on the number of commodities per a given agency.

    .. figure:: images/commoditiesPerAgency.png



.. note::

    A future version of this server may add support for social authentication
    e.g login via Facebook, Twitter or Google accounts.


.. toctree::
    :maxdepth: 4
