
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

<img width="679" alt="Screenshot 2023-11-05 at 8 37 35 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/b2a7f04b-f891-4ed4-a98a-70141c8d3b1f">


## Data Dictionary :
<img width="881" alt="Screenshot 2023-11-05 at 8 28 52 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/95f0933c-d140-4b66-847f-ae79ef2b1b12">

<img width="899" alt="Screenshot 2023-11-05 at 8 29 26 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/7d4e0503-4d23-44e0-84ef-82166a59b8c1">

<img width="891" alt="Screenshot 2023-11-05 at 8 29 49 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/8c3803fe-694f-4e44-9548-36558bdfdb4d">

<img width="887" alt="Screenshot 2023-11-05 at 8 30 13 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/31ac9788-2983-49a8-94bd-71980eb70f31">

<img width="898" alt="Screenshot 2023-11-05 at 8 30 33 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/c7c35aa6-5b5b-470c-b4af-769ae81741fe">

<img width="882" alt="Screenshot 2023-11-05 at 8 30 58 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/9ab385f8-689d-4bb8-904c-62d7cba0accf">

<img width="889" alt="Screenshot 2023-11-05 at 8 31 20 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/49c26d69-077f-42bc-bd26-c7853052f953">

<img width="893" alt="Screenshot 2023-11-05 at 8 31 42 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/d7f9fda6-ef93-43f2-8d03-51f5abe96a82">

<img width="900" alt="Screenshot 2023-11-05 at 8 32 07 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/ac1db01a-b21c-4529-a892-f810c066b815">

<img width="889" alt="Screenshot 2023-11-05 at 8 32 42 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/3ba2d3ba-e617-4987-8c66-1f7fdadc8c1b">

<img width="892" alt="Screenshot 2023-11-05 at 8 34 58 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/0f73cacb-5385-435d-a78d-39a43fec9eb7">

<img width="902" alt="Screenshot 2023-11-05 at 8 35 48 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/b066392d-cd65-48ec-8dda-1a63705de79d">





## Queries :
<img width="896" alt="Screenshot 2023-11-06 at 3 22 09 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/5d3a70eb-f945-4bca-b58f-7404892b47af">

1. Query 1 lists all players that have not suffered any injuries. This query lists each player's first and last name, and their team name.

<img width="1002" alt="Screenshot 2023-11-06 at 3 27 26 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/6a6c0afc-a841-4ff5-a493-f89e7a34f415">

 From a managerial perspective, this query would be important because knowing what players have not been injured in the past and whether or not they are currently injured or not would be significant in understanding the state of the team and help predict how they would fare in a tournament. For a team that has many injured players it would not be wise to send them to participate in a tournament because they wouldn’t be able to perform on a competitive level with many injured players. 

2. Query 2 lists the names of the teams and their respective head coaches that won a tournament:

<img width="935" alt="Screenshot 2023-11-06 at 3 32 02 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/3005dc0a-415d-458d-abb7-e2a1417be5c7">
 
 The manager would want to know who the head coach is for every team that won the different tournament. This would be important that the manager was aware of which coaches were in charge of the overall winners of the four tournaments. 

3. Query 3 lists the first and last name of each player on the Lions team. 

<img width="1111" alt="Screenshot 2023-11-06 at 3 35 59 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/af6165df-e3fd-4820-bc44-f6705d58af40">

This information would be important for a manager who is interested in the Lions team and wants to know who each player is in order to do research on the stats of each player.

4. Query 4 lists the team names that played in the S.M.A.S.H tournaments and then orders those teams alphabetically.

   <img width="1082" alt="Screenshot 2023-11-06 at 3 40 46 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/3a8016e4-9aff-4bb0-b393-e21d98abc799">

This query is important from a managerial perspective because the S.M.A.S.H. tournament was the last one of the season. It is important to see which teams practiced the longest before playing in any tournaments to compare performance evaluations.

5. Query 5 lists lists out the name and the payment of those sponsors whose payment amount is greater than the average payment amount made by all the sponsors.

<img width="1079" alt="Screenshot 2023-11-06 at 3 43 08 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/9bbbf769-0f60-4997-b746-4d6314847148">

A manager would want to know this information because it would show which sponsors are the most generous in comparison to the rest. The sponsors that donate the most money would be put on the jerseys of the players. 

6. Query 6 lists the first name and last name of the referees of each match played by the bulldogs. 

<img width="1083" alt="Screenshot 2023-11-06 at 3 45 50 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/45d11f27-af88-49ab-8033-2c6c5490a8df">

A manager would want to know this information to determine if the bulldogs are cheating so they want to know the referees in order to contact them.

7. Query 7 lists all the staff that are maintenance workers at facilities with field conditions that are turf.
   <img width="1084" alt="Screenshot 2023-11-06 at 3 47 40 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/5f62b610-7af4-4a53-9150-46c6edc70d35">

   This query would be significant to a manager who would want to understand how many maintenance workers are at a particular facility that has turf.

8. Query 8 shows the average number of years of experience coaches have for each team where the number of years of experience is greater than 15.

   <img width="1065" alt="Screenshot 2023-11-06 at 3 49 35 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/f3b36ada-865e-4348-93a3-fa1c9ca0696f">

The manager would want to know this information to understand the individual experience of each coach and which teams have coaches with the most experience. This would allow the manager to assign head coaches to competition levels that are appropriate for their experience level. Coaches with more coaching experience should be assigned to higher competition levels, and the opposite could be said for coaches with less experience. 

9. Query 9 shows the first and last name of each individual coach that has no coaching  certification along with the team that they coach for.

<img width="1078" alt="Screenshot 2023-11-06 at 3 51 19 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/e8497dfb-7dc6-454f-baf9-d6eb52f91937">

The owner of the Bulldog United soccer club would want to know this information to track each coach’s progress towards obtaining their coaching certification. This would be relevant when coaches are up for evaluation and would help in determining what coaches would be qualified to become a head coach of a team for the upcoming season. 

10. Query 10 shows the name of the tournament that had an average amount of payments that was higher than the average total amount of payments from all sponsors.

<img width="1084" alt="Screenshot 2023-11-06 at 3 52 46 PM" src="https://github.com/ashley-potts/MIST-4610-Project1/assets/148247835/7f10ee5c-5428-42f8-a98b-316e4764175b">

A manager would be interested in this information to determine which tournament had the highest amount of money from its sponsors. It would help them see which tournament was the biggest, most profitable event to these sponsors. This particular tournament had a group of teams that brought money in from some of the highest paying sponsors. 


## Database Information : 
The name of the database is : cs_g10p1
Each query created is marked in the database using stored procedures. The stored procedures can be called using the following format : CALL Q1();
