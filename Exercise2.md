# Database
## Exercise 2: Single Table Queries
### Task 1
    select * from goal;
<img width="1440" alt="screenshot-task1" src="https://github.com/user-attachments/assets/c1afc559-f450-41cb-823e-e12279b5f22a">


### Task 2
    select name,type from airport where iso_country='FI';
<img width="1440" alt="screenshot-task2" src="https://github.com/user-attachments/assets/9e31282d-a533-4f36-94a7-0705150c7b49">


### Task 3
    select name from airport where iso_country='FI' order by name asc;
<img width="1440" alt="screenshot-task3" src="https://github.com/user-attachments/assets/d396fdc3-05b2-485a-ba5b-9c45d9a45a00">


### Task 4
    select name,type from airport where iso_country='FI' order by type asc, name asc;
<img width="1440" alt="screenshot-task4" src="https://github.com/user-attachments/assets/1b95d6dd-2c06-469b-b2bb-e5a4213287cb">


### Task 5
    select name from country where name like 'F%';
<img width="1440" alt="screenshot-task5" src="https://github.com/user-attachments/assets/2a1207b4-d0a5-479b-8175-901cf5e8cdc6">


### Task 6
     select name from country where name like '%F%';
<img width="1440" alt="screenshot-task6" src="https://github.com/user-attachments/assets/906e389e-f561-4afe-a6b5-90eaef7547b9">


### Task 7
    select location from game where screen_name="Vesa";
<img width="1440" alt="screenshot-task7" src="https://github.com/user-attachments/assets/6d1f8be4-fbd3-4940-b917-4ef2ee9b0631">


### Task 8
    select co2_consumed from game where screen_name='Ilkka';
<img width="1440" alt="screenshot-task8" src="https://github.com/user-attachments/assets/c0eda4ae-f206-4079-8ada-3cd9c37f1a66">

### Task 9
    select co2_budget from game limit 1;
<img width="1440" alt="screenshot-task9" src="https://github.com/user-attachments/assets/c01c1073-103b-4a19-afa5-5e0f634f1ece">


### Task10
    select screen_name,co2_budget,co2_consumed,@co2_left :=co2_budget - co2_consumed as co2_left from game where screen_name='Ilkka';
<img width="1440" alt="screenshot-task10" src="https://github.com/user-attachments/assets/c1c5b9cc-c9c1-4384-991d-210bbf3eaed8">
