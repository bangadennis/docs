Installation Process
=====================

Introduction
-------------
Linux-Ubuntu server is the preferred development and deployment environment for this application. 

The Dependencies-Development and Production environment required are:

#. Git- This is a distributed revision control system.

#. MySQL  database(>5.5), apache server and php(>=5.3)-LAMP.

#. php-curl.

#. crontab.


Installation
-------------

#. Install all the depencies i.e the ones listed above in your machine.

#. Clone the application from the github repository to your document root in your machine/Or Copy the application folder into your document root.

.. note::

    Please note that you must have an account on Github in order to do this.


Setup and Configuration
------------------------

#. Create a mysql database from your localhost and dump the database schema  into it.( Database Schema is in  the application’s root folder).

#. In the *config.php* file (application_name/system) change the configurations for:

  * MySQL Database name.

  * MySQL user and the MySQL password.

  * Base path for your application.

  * DHIS2 url

  * DHIS2 access username and password for api interaction. 


3. Setup a cronjob to download data elements from DHIS2.(Executes hourly).

  * api/download_dataElements.php










.. toctree::
    :maxdepth: 2
