WEEK 4 Exercise: 4

Qno.1 ans
select country.name as "country name ", airport.name as "airport name" from country inner join airport on country.iso_country = airport.iso_country where country.name = "Finland" ;


![4-1](https://github.com/user-attachments/assets/c46c013f-e991-4980-b8b6-691132ecedea)


Qno.2 ans

 select screen_name, name from game inner join airport on game.location = airport.ident;

 
![4-2](https://github.com/user-attachments/assets/dac39dce-89f1-4a8e-a310-6a5d9003130e)


Qno.3 ans

select game.screen_name, country.name from game inner join airport on game.location = airport.ident inner join country on airport.iso_country = country.iso_country;


![4-3](https://github.com/user-attachments/assets/88fff21e-f8c9-4056-a282-af632403f643)


Qno.4 ans

select name, screen_name from airport left join game on game.location = airport.ident where name like "%Hels%" order by screen_name desc;


![4-4](https://github.com/user-attachments/assets/71950ac6-8c42-4cad-a501-b2cd045b430c)


Qno.5 ans

 select name, screen_name from goal left join goal_reached on goal.id = goal_id left join game on game.id = game_id;
 

![4-5](https://github.com/user-attachments/assets/6fc0202f-b6b6-4883-b305-9d8b9bbba530)


