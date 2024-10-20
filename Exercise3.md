#  Week 3
## Exercise 3: Multiple Table Queries
### Task 1
    select country.name as 'country name', airport.name as 'airport_name' from country,airport where country.iso_country = airport.iso_country and country.name = 'Iceland';
  
  <img width="1440" alt="screenshot_task1" src="https://github.com/user-attachments/assets/b5501a48-f4b4-4752-ba4d-12a6082e9025">

### Task 2
    select airport.name as 'airport name' from airport,country where airport.iso_country = country.iso_country and country.name = 'France' and airport.type='large_airport';
    
  <img width="1440" alt="screenshot_task2" src="https://github.com/user-attachments/assets/a8843ae7-5b1d-437a-b223-675c4e138000">

### Task 3
    select country.name as country_name,airport.name as airport_name 
    -> from airport,country
    -> where airport.iso_country = country.iso_country
    -> and country.continent ="AN";
    
  <img width="1440" alt="screenshot_task3" src="https://github.com/user-attachments/assets/72d6cd53-2809-41a2-9092-f01bf9d20676">

### Task 4
    
    select airport.elevation_ft as elevation_ft 
    -> from airport,game
    -> where airport.ident = game.location
    -> and game.screen_name = "Heini";

  <img width="1440" alt="screenshot_task4" src="https://github.com/user-attachments/assets/b1fecf79-16a6-4ce4-86f5-1dbb54ac8382">

### Task 5
    select elevation_ft*0.3048 as elevation_m from airport,game where location = ident and screen_name ="Heini";
  
  <img width="1440" alt="screenshot_task5" src="https://github.com/user-attachments/assets/13633408-3aca-4df6-a5b4-fee499c50b07">

### Task 6
    select name from airport,game
    -> where ident = location
    -> and screen_name="Ilkka";

  <img width="1440" alt="screenshot_task6" src="https://github.com/user-attachments/assets/96d94d45-42d6-4dff-adfd-507f80dbd560">
   

### Task 7
    select country.name
    -> from airport,game,country
    -> where location = ident
    -> and airport.iso_country=country.iso_country
    -> and screen_name="Ilkka";

  <img width="1440" alt="screenshot_task7" src="https://github.com/user-attachments/assets/201ccf9a-68b8-4600-a360-0207b3e6c1b5">

### Task 8
    select name from goal,goal_reached,game
    -> where game.id=game_id
    -> and goal.id=goal_id
    -> and screen_name="Heini";
    
  <img width="1440" alt="screenshot_task8" src="https://github.com/user-attachments/assets/950eee56-3738-4ff2-9c0a-46ffe32fea57">
   

### Task 9
    select airport.name 
    -> from airport,game,goal,goal_reached
    -> where ident = location
    -> and goal.id = goal_id
    -> and game.id = game_id
    -> and screen_name = "Ilkka"
    -> and goal.name = "CLOUDS";

  <img width="1440" alt="screenshot_task9" src="https://github.com/user-attachments/assets/99811a72-5ab9-49df-bede-6272e8fd1c02">

   
### Task10
    select country.name
    -> from airport,country,game,goal,goal_reached
    -> where ident = location
    -> and airport.iso_country = country.iso_country
    -> and game.id = game_id
    -> and goal.id = goal_id
    -> and screen_name = "Ilkka"
    -> and goal.name = "clouds";
    
  <img width="1440" alt="screenshot_task10" src="https://github.com/user-attachments/assets/bbd9aadd-ad73-45a0-a245-02c8610a5da5">


   
