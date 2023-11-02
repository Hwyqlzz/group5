<h1>GROUP 5 MIST 4610 Group Project 1</h1>
<h2>TEAM NAME:</h2>
29704 Group5
<h2>Team Members:</h2>

1. Michael Hearnes [@michaelhearnes](https://github.com/mh101410)

2. Elton Hsieh [@eltonhsieh](https://github.com/ehsieh1)

3. Aidan Kane [@aidankane](https://github.com/aidanpatrickkane)

4. Mandy Larsen [@mandylarsen](https://github.com/awl25)

5. Zhengze Li [@zhengzeli](https://github.com/Hwyqlzz)

6. Nabeel Mohammed [@nabeelmohammed](https://github.com/nabeelmohd56)

<h2>Problem Description:</h2>
Our project creates a relational database for a tennis club based on the prompt entered below into ChatGPT. In this case, ChatGPT acted as the client and set the appropriate entities and attributes for us to model as necessary. 

Prompt: Pretend you are the owner/operator of a tennis (or football, soccer - your choice) club
needing to build a relational database. You hired some students from the MIST 4610 class at
the University of Georgia to create the database for you. They need to know more about your
organization to identify which entities, attributes, and relationships are important for you.
Start by describing your business as a real client.

Response: I am the owner/operator of a tennis club called "Green Valley Tennis Center," located in Athens, Georgia. Our club is a premium tennis facility that caters to tennis enthusiasts of all ages and skill levels. We offer a range of services, from professional coaching and training to court rentals, leagues, tournaments, and a pro shop. Our goal is to provide a top-notch experience for tennis players and create a vibrant and welcoming tennis community in our area.

Key aspects of our business that the MIST 4610 class students should consider when designing the relational database include:

1. **Memberships**: We offer different types of membership plans, including monthly, annual, and family memberships. Each membership type may have varying access levels and associated fees.

2. **Court Reservations**: Members and non-members can reserve tennis courts for specific dates and times. The reservation system needs to handle bookings, cancellations, and court assignment.

3. **Player Profiles**: We maintain profiles for all our members and track their personal information, contact details, and skill levels. Players can have multiple addresses and phone numbers, and we keep a record of their preferred contact methods.

4. **Coaching and Instruction**: We have a team of certified tennis coaches who offer private and group lessons. The database should track coach profiles, their availability, and coaching schedules.

5. **Pro Shop Inventory**: We sell tennis equipment and apparel in our pro shop. The database should manage inventory levels, product details, and sales records.

6. **Leagues and Tournaments**: We organize various tennis leagues and tournaments throughout the year. The database should handle registrations, match schedules, and results.

7. **Billing and Payments**: We bill members for their memberships and other services. The database should record billing history, payment methods, and outstanding balances.

8. **Communication**: We send out newsletters and event announcements to our members. The database should manage contact lists and communication preferences.

9. **Employee Records**: We employ staff for court maintenance, front desk operations, and coaching. Employee records should include personal information, job roles, and work schedules.

10. **Feedback and Surveys**: We collect feedback from members to continuously improve our services. The database should store survey responses and feedback history.

11. **Security and Access Control**: Different users (members, employees, administrators) may have varying levels of access to the system. The database should support role-based access control.

12. **Reporting and Analytics**: We need to generate reports on membership statistics, court usage, revenue, and more to make informed business decisions.

The students from the MIST 4610 class should consider these aspects when designing the database schema, identifying the entities (tables), their attributes (fields), and the relationships between them. The relational database should facilitate efficient management of our tennis club's operations and help us deliver a seamless experience to our members and guests.

Based on this response from the client, we determined that the entity central to the data model are the tennis clubs. Players can then buy memberships, participate in tournaments and leagues, reserve courts, and book lessons with coaches. Additionally, each club has a pro shop with merchandise, from which players can place orders. All employees of the club are modeled as well, including support staff and tennis coaches. The goal of our database is to model the entities and their respective attributes, the relationships between them, and then to create sample data off of which the tables can be populated. This will allow us to write SQL queries on the database that will provide us with insight into the operations of the club.

<h2>Data Model:</h2>

Explanation of data model:

Data model:
![IMG_2808 13](https://github.com/Hwyqlzz/group5/assets/148079593/1d81de7c-b9ac-4bf7-8bcc-b3fcdb0a38b2)

<h2>Data Dictionary:</h2>

<img width="601" alt="employees" src="https://github.com/Hwyqlzz/group5/assets/35616163/79dd32bc-c1dc-4396-b941-1096876cd8e9">







<h2>Queries:</h2>

Query 1: lists out the playerID, player name, and the number of court reservations per player.
<img width="1092" alt="Screenshot 2023-11-01 at 16 51 05" src="https://github.com/Hwyqlzz/group5/assets/148079593/34efbe54-b542-4311-ba3b-806d3accc9f8">

This will allow the club to recognize how many times a player has made a reservation, allowing for some packages or discounts to be offered to those with more bookings.

Query 2: lists a query that lists the information for all the players who have not made a court reservation.
<img width="1064" alt="Screenshot 2023-11-01 at 16 51 43" src="https://github.com/Hwyqlzz/group5/assets/148079593/7b91476c-6cc8-4c33-8eb6-29d9d53f4148">
This allows the club to market to and contact specific customers ( promotional emails or coupons). This helps to maximize revenue and efficiency as it specifically targets those who are not engaged in the booking rather than wasting time and resources advertising to those who are already engaged in the booking.

Query 3:  lists out the player name and number of lessons, it’s a simple query.
![elton hsieh simple query 3 93](https://github.com/Hwyqlzz/group5/assets/148079593/569b3b09-a690-4c01-875d-253ce9c59713)


It allows the club to track which players have made lessons to keep into their logs.

Query 4:  lists out % of players and coaches who identify as either “non-binary” or “prefer not to say” and it’s a complex query.  
![elton hsieh complex query 4 46](https://github.com/Hwyqlzz/group5/assets/148079593/acada3c7-c069-4ce3-8c45-37307516c69c)


It allows the club to see what percentage of their players and coaches prefer to have complete gender neutrality.

Query 5:  lists out the player names who have spent less on merchandise than the average player, it’s a complex query.  
![aidan complex query 5 78](https://github.com/Hwyqlzz/group5/assets/148079593/95e30d27-d07b-4eec-95b7-ddfb1e0d6759)


It allows the club to keep track of who are their most loyal players, and who aren’t.

Query 6:  lists out players who have never played in a tournament, it’s a simple query.  
![aidan simple query 6 50](https://github.com/Hwyqlzz/group5/assets/148079593/aa16ac8b-3a09-4c70-9fe9-39b564154be4)


It allows the club to market who are making their opening debut in which tournaments, and may garner a larger audience.

Query 7

Query 8

Query 9

Query 10

<h2>Database information:</h2>
Name of the database: ns_F2329704Group 5

Additional information: All queries above are stored as procedures in the database and are callable using the format: CALL TP_Q1();

