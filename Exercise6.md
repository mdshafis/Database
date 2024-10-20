## Exercise 6: Aggregate queries

# Task1

    select elevation_ft from airport where elevation_ft in(select max(elevation_ft) from airport);
    
<img width="1440" alt="screenshot_task1" src="https://github.com/user-attachments/assets/25a0ac4b-53f7-4f17-b47b-8d41a1f42ccd">

# Task 2:

    select continent, count(*) from country group by continent;

<img width="1440" alt="screenshot_task2" src="https://github.com/user-attachments/assets/237b8395-8a07-4e2a-88d9-adff02e5883d">

# Task 3:

  select screen_name, count(*) from game, goal_reached where id = game_id group by screen_name;

<img width="1440" alt="screenshot_task3" src="https://github.com/user-attachments/assets/bb8fc982-cc98-4d7c-abaa-0d59ff2ab3a0">

# Task 4:

  select screen_name from game where co2_consumed in (select min(co2_consumed) from game);

<img width="1440" alt="screenshot_task4" src="https://github.com/user-attachments/assets/e12d2732-48a6-49c7-9961-4d1a29093189">

# Task 5:

  select country.name, count(*) from airport, country where airport.iso_country = country.iso_country group by country.iso_country order by count(*) desc limit 50;

<img width="1440" alt="screenshot_task5" src="https://github.com/user-attachments/assets/72b6d6e0-9653-44e0-87e7-f2afd09dfc46">

# Task 6:

  select country.name from airport, country where airport.iso_country = country.iso_country group by country.iso_country having count(*) > 1000;
  
<img width="1440" alt="screenshot_task6" src="https://github.com/user-attachments/assets/d1f27788-63f3-4ed9-82d9-5f5609006222">

# Task 7:

 select name from airport where elevation_ft in(select max(elevation_ft) from airport);

<img width="1440" alt="screenshot_task7 " src="https://github.com/user-attachments/assets/2e7d185d-449c-4b93-9d1a-400614422740">

# Task 8:

  select name  from country where iso_country in( select iso_country from airport where elevation_ft in( select max(elevation_ft) from airport));

<img width="1440" alt="screenshot_task8" src="https://github.com/user-attachments/assets/013f4c70-5c5f-4f69-accc-19278252a0ce">

# Task 9:

  select count(*) from game, goal_reached where id = game_id and screen_name = "Vesa" group by screen_name;

<img width="1440" alt="screenshot_task9" src="https://github.com/user-attachments/assets/42515636-954f-41ec-a333-6d520314b62c">

# Task 10:
  select name from airport where latitude_deg in( select min(latitude_deg) from airport );

<img width="1440" alt="screenshot_task10" src="https://github.com/user-attachments/assets/12c94907-cdd1-4d64-a8b9-e257d5d6209b">








 






