
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

## Database Information : 
The name of the database is : cs_g10p1
