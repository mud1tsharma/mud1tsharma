This folder contains the following files:

- ### 1 Data Cleaning.sql
  
  - SEARCHING FOR ERRORS
    - Search for duplicate primary keys in all tables
    - Search for illegal foreign keys
    - Search for illegal dates
    - Search for misclassified data
    - Search for miscalculated data
  
  - RECTIFYING ERRORS
    - Instantiate tables with unique primary keys
    - Remove or replace invalid foreign keys
    - Remove or replace illegal dates (Eg. A hire ended before it began)
    - Remove or replace illegal or invalid classifications (Eg. earthmoving equipment was misclassified as sports equipment)
    - Recalculate calculated fields to ensure validity (Some business rules were incorrectly applied)

- ### 2 Implement a Data Warehouse.sql
	- Identify dimensions, attributes, and fact measures
	- Create the relevant dimension tables
	- Create temporary fact tables to add calculated fields (Eg. Seasons, Type of Sale; low, medium, or high)
	- Create a final fact table

- ### 3 OLAP Queries.sql
	- Top n, and Top n% involving:
		- 2 attributes from 2 different dimensions
		- 1 fact measurement
	- Subtotals using CUBE, ROLL-UP, and/or PARTIAL ROLL-UP
	- Moving and cumulative aggregates
	- Partitions		
