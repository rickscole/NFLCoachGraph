# NFLCoachGraph
Files related to creating and analyzing graph structure of coaches/personnel in the National Football League

Includes the following steps
- Use of webcrawler (via R Script) to scrape organizational information for each NFL Team - Year from wikipedia
- With some modifications, the resultant output dataframe from above is saved to a .txt and imported into a SQL Server environment (currently a local DB, though the plan is to migrate to Azure when this project is on more solid footing)
- Table from above combines with pre-defined ontological structure (also stored in SQL Server) and other query elements (for data scrubbing / integrity purposes) to create final weighted, directed edge list
- Weighed, directed edge list is saved to a CSV, and imported into Python
- Graph analysis done in Python using igraph library
