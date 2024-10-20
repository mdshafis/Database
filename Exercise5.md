## Exercise 5: Subqueries
# Task 1:

    select country.name from country where country.iso_country in ( select airport.iso_country from airport where name like 'Satsuma%' );
    
<img width="1440" alt="screenshot_task1" src="https://github.com/user-attachments/assets/9560ce78-2e32-43c2-b421-b8b49bdc93c1">

# Task 2:
    
    select name from airport where iso_country in(select iso_country from country where name = "Monaco");
    
<img width="1440" alt="screenshot_task2" src="https://github.com/user-attachments/assets/d83df947-68b6-49df-9d69-5e39dbcecaac">

# Task 3:

    SELECT screen_name FROM game WHERE id IN (SELECT game_id FROM goal_reached WHERE goal_id = (SELECT id FROM goal  WHERE name = 'CLOUDS';

<img width="1440" alt="screenshot_task3" src="https://github.com/user-attachments/assets/e8961a2c-1d91-4c42-aeff-c4257a79a726">

# Task 4:

    SELECT name FROM country WHERE iso_country NOT IN (SELECT iso_country FROM airport );
    
<img width="1440" alt="screenshot_task4" src="https://github.com/user-attachments/assets/6df41812-72e0-4132-a67a-dc54f1b944d2">

# Task 5:

    select name from goal where id not in( select goal.id from goal, goal_reached, game where game.id = game_id and goal.id = goal_id and screen_name = "Heini" );

<img width="1440" alt="screenshot_task5" src="https://github.com/user-attachments/assets/15c6c163-a96f-4a19-bb01-bf31aae4bb38">







    
