# Exercise 7: update queries

## Task 1: 

  update game set location = (select ident from airport where name = "Nottingham Airport"), co2_consumed = co2_consumed+500 where screen_name = "Vesa";
  select * from game;
  
<img width="1440" alt="screenshot_task1" src="https://github.com/user-attachments/assets/8ffe38f1-b2a6-463f-843b-8c5333ac8313">

# Task2 : Prepare your own database for the project by deleting all dummy data relating to the game state. To maintain referential integrity, you have to delete the data in a specific order. 
# Do you have to delete data first from the game table or from the goal_reached table?
    goal_reached

## Task 3:

  delete from goal_reached;
  select * from goal_reached

<img width="1440" alt="screenshot_task3" src="https://github.com/user-attachments/assets/82b1b845-9a09-41fe-b36a-153ea18d8972">

## Task 4:

  delete from game;
  select * from game;
  
<img width="1440" alt="screenshot_task4" src="https://github.com/user-attachments/assets/6a144ec1-c454-43a4-9ca3-31b48e35b841">


