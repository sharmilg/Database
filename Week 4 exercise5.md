WEEK 4 Exercise: 5

Qno.1 ans

select name from country where iso_country in(select iso_country from airport where name like "Satsuma%");


![4 2-1](https://github.com/user-attachments/assets/3fc54003-f628-4ed7-907a-316c7893a3ac)


Qno.2 ans

select name from airport where iso_country in(select iso_country from country where name ="Monaco");


![4 2-2](https://github.com/user-attachments/assets/0cda98b0-f33b-4d5e-b321-1076630c57ab)


Qno.3 ans

select screen_name from game where id in(select game_id from goal_reached where goal_id in(select id from goal where name ="CLOUDS"));


![4 2-3](https://github.com/user-attachments/assets/1ef8b078-fafa-498e-afb0-089663af0619)


Qno.4 ans

select country.name from country where iso_country not in(select airport.iso_country from airport);


![4 2-4](https://github.com/user-attachments/assets/b3dcfc9c-9e39-41e4-b844-706989a858bb)


Qno.5 ans

select name from goal where id not in(select goal.id from goal, goal_reached, game where game.id= game_id and goal.id = goal_id and screen_name like 'Heini%');


![4 2-5](https://github.com/user-attachments/assets/f9d0e171-d9a8-4b47-b696-921e8f8e988e)
