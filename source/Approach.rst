Approach
============================

The project is developed as a DHIS2 Web APP.


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
to being presented with all the facilities at once.

Once the Central stores, dispensing points, satellite sites and stand alone sites
are established and inserted into the database, DHIS2 Web API is queried for 
analytics based on the hierarchy established and the results displayed.



.. toctree::
    :maxdepth: 2
