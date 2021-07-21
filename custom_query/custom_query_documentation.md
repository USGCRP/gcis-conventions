The custom query tool is an intuitive search functionality that provides a GCIS user with the means to develop simple search queries with downloadable results in the form of a data table. It uses an SQL-type syntax with limited scope: the tool is built around the SQL SELECT, FROM, and WHERE statements, with allowance to specify a wide range of GCIS resource attributes. However, rather than type query statements, a user develops a query by selecting options from drop-down menus.  

The custom query tool advances search functionality that goes beyond the limitations of the “search bar” in the GCIS website. Importantly, it helps a user develop a query in a stepwise fashion. Also, given the several and sometimes unique attributes belonging to each GCIS publication, the custom query tool simplifies querying by displaying only those attributes relevant to the GCIS publication specified in the first drop down menu. These features are described below.

Step 1: To develop a query, first start by specifying the initial publication (for example, “Reports”). Like all other input specifications, this can be done by selecting the relevant data table from the drop-down menu.
Step 2: Specify one or more attributes (for example, “identifier”) of the selected table to filter by. Only attributes relevant to the publication selected in Step 1 will be displayed. 
Step 3: Select a relationship option for the selected publication (for example, “having”).
Step 4: Select a secondary publication to query against (for example, “images”).
Step 5 (optional): Specify attributes for the WHERE statement in similar fashion as described above. 

The above query would read “SELECT Title FROM Report HAVING Image”.
