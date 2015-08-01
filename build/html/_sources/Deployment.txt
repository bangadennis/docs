Approach
============================

The project is developed as a DHIS2 Data Aggregation WebApp that would run on an independent instance and maintain its own local database, but have the ability to read and write to DHIS2.


The web API and the database
----------------------------

The Web API is used to a great deal as a source of data for the backborne database
used. The API allows us to query for all organization units and sort them into
Counties (Level 2), SubCounties (Level 3) and facilities (Level 4). This data is
then used to populate the respective tables in the database.

Once all this data is inserted into the database, the process of establishing which
facilities lie under which category begins. This is left to the discretion of the
user who is prompted to supply facilities under each category from the list we have.

The purpose of incorporating the existing DHIS2 hierarchy of counties and sub-
counties is to aid the user in the search and selection process by providing a
mechanism in which they can drill down to a smaller number of facilities as opposed
to being presented with all the facilities at once e.g 

* the user should be able to generate a combined report (MoH730A or MoH729A) for the Sub-county store and its Satellite sites.



* the user should also be able to group Standalone sites by county or sub-county (or Central sites or Sub-county stores). 


Once the Central stores, dispensing points, satellite sites and stand alone sites
are established and inserted into the database, DHIS2 Web API is queried for 
analytics based on the hierarchy established and the results displayed.



.. toctree::
    :maxdepth: 2
