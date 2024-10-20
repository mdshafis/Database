# Exercise 4: Join
## Task 1
    select country.name as "country name", airport.name as "airport name" from country inner join airport on airport.iso_country = country.iso_country where country.name = "Finland" and scheduled_service = "yes";
    
<img width="1440" alt="screenshot_task1" src="https://github.com/user-attachments/assets/84fa2598-1cfd-469d-9076-b6f39846aecb">

## Task 2
    select game.screen_name,airport.name from game inner join airport on airport.ident = game.location;
    
<img width="1440" alt="screenshot_task2" src="https://github.com/user-attachments/assets/6754b32a-bb48-4899-b534-80ece8edef60">

## Task3 
    select game.screen_name,country.name from game inner join  airport on airport.ident = game.location inner join country on country.iso_country = airport.iso_country;
    
<img width="1440" alt="screenshot_task3" src="https://github.com/user-attachments/assets/aff50ab4-8962-44a9-9ab9-41bae5f07c0d">

## Task 4
    select airport.name, screen_name from airport left join game on ident = location where name like "%Hels%";
    
<img width="1440" alt="screenshot_task4" src="https://github.com/user-attachments/assets/77db889b-938e-4e88-998b-faa7a028bade">

## Task5
    select name, screen_name from goal left join goal_reached on goal.id = goal_id  left join game on game.id = game_id;
    
<img width="1440" alt="screenshor_task5" src="https://github.com/user-attachments/assets/958674b3-d472-4940-a3a0-ca2edc1d7f39">
 



