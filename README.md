
MIST 4610 Group Project 1 
## Team Name : 
Group 10

## Team Members :
1. Ashley Potts @ashley-potts
2. Emma Surbrook @emmasurbrook
3. Hayden Soley @HaydenSoley
4. Liam Kilner @liamkilner
5. Victoria Wiest @victoriawiest

## Problem Description :
The current project is to create a relational database that models the general operations of a soccer club. The primary entity of the model is the Teams entity with the Teams representing each individual team that belongs to the UGA United Soccer Club. The Team entity has various relationships with other entities in the model such as Players, Coaches, Tournaments, etc. We are interested in accurately depicting these relationships and generating sample data to ensure that the goals of the database are achieved. Additionally we plan to execute queries on the sample data to provide information that is relevant to the club from a managerial perspective. 
## Data Model
Our model is based on a Soccer Club, called UGA United Soccer Club. Our “Teams” table serves as our central entity, branching to many other tables throughout the model. “Teams” includes many important attributes, such as team name, age group, and practice schedules. Our “Teams” table has a one-to-many relationship, as well as a one-to-one relationship with our “Coaches” table. There are many coaches per team, with one being the head coach, shown by the one-to-one relationship. Our “Coaches” table gives important information about each coach, such as name, contact information, and coaching experience. Additionally, “Teams” links, as a one-to-many relationship, to “Registration”. There are many registrations per team. There is also one player per registration. Our “Registrations” entity as a one-to-one relationship with “Players”. This table includes information such as name, age, contact information, and emergency contacts. “Teams” continues its relationships by having a one-to-many relationship with “Sponsors”. Each team can have multiple sponsors, each of different levels and payments. There is also a one-to-many relationship between “Teams” and “Tournaments”. Each tournament is linked to multiple teams. This table includes important information such as the name, location, and date of the tournaments, as well as the winning team. Our “Tournaments” entity branches to “Facilities”, with multiple facilities as a part of each tournament. Our facilities offer different field conditions, such as turf or grass, and multiple fields within the facility. The “Facilities” entity also links to our “Staff” entity through a one-to-many relationship. Each facility has multiple staff members, where we can find information about their contact information and position. The “Tournaments” entity also links to another entity, “Matches”, through a one-to-many relationship. There are multiple games in each tournament, and also multiple referees in each match. This is shown by the “Matches” and “Referees” entities being connected with a one-to-many relationship. Our “Teams” entity connects to one more entity, “Practice Sessions”, through a one-to-many relationship since there are multiple practice sessions for each team. Since many facilities can have many practice sessions, there is an associative entity between “Practice Sessions” and “Facilities” called “Practice_Sessions_has_Facilities”. This shows which practice sessions are occurring at each facility. 


## Data Dictionary :

## Queries :
Include a natural language description of the query and a justification as to why each query is
relevant from a managerial perspective (why would a manager be interested in the query
results). Avoid having queries that are almost identical to one another. Add the written of the
query as well as the response (e.g., copy and paste Execute to Text) of each query. You can also
use the code markdown to highlight the SQL code and copy and paste the results into the file.
To ensure the complexity of the queries some of the things that may be considered include
multiple table join, traditional subquery, correlated subquery, GROUP BY, GROUP BY with
HAVING, multi condition WHERE, Built-in functions (e.g., AVG) or a calculated field, REGEXP,
NOT EXISTS, and more.
You may combine some of the preceding list of features into a single query (still have to provide
10 queries). Indicate in matrix format in your report which features are covered in a query
## Database Information : 
The name of the database on the MySQL server. Each table should be populated with enough
data so that the queries return a sufficient result set. All queries should be bookmarked
through the use of stored procedures (take a look at the example on ELC) according to this
format: TP_Qx (where x is to be replaced by the query number)

The name of the database is : cs_g10p1
