Week 5 Exercise-6

Qno.1 ans

Select max(elevation_ft) From airport;


![6-1](https://github.com/user-attachments/assets/a8852984-a5e7-4431-ab31-800d2f9733ec)


Qno.2 ans

select continent, count(*) from country group by continent;


![6-2](https://github.com/user-attachments/assets/35000f05-24c9-4bce-879b-fdc07e010bc7)


Qno.3 ans

select screen_name, count(*) from game, goal_reached where id = game_id group by screen_name;


![6-3](https://github.com/user-attachments/assets/fddac686-b8ed-4b96-aa4d-b8f286991dea)


Qno.4 ans

select screen_name from game where co2_consumed in (select min(co2_consumed) from game);


![6-4](https://github.com/user-attachments/assets/0bfe4b71-1be2-471a-a8ec-4c8c45c8153b)


Qno.5 ans

select country.name, count(*) from country inner join airport on airport.iso_country = country.iso_country group by country.name order by count(airport.id) desc limit 50;


![6-5](https://github.com/user-attachments/assets/643ef3c0-c8e3-4afb-bc9b-543dfbb561e2)


Qno.6 ans

select country.name from country inner join airport on airport.iso_country = country.iso_country group by country.name having count(airport.id) > 1000;


![6-6](https://github.com/user-attachments/assets/8eef2c9c-1909-4a4d-9c6b-70bfd7675018)


Qno.7 ans

select name from airport where elevation_ft in (select max(elevation_ft) from airport);


![6-7](https://github.com/user-attachments/assets/94ebe32a-1683-4622-8acf-93abe085741d)


Qno.8 ans

select country.name from country inner join airport on airport.iso_country = country.iso_country where elevation_ft in (select max(elevation_ft) from airport);


![6-8](https://github.com/user-attachments/assets/b849cc95-d3f1-4e9a-ba3a-416682d5e2a9)


Qno.9 ans

select count(*) from goal_reached, game where id = game_id and screen_name = "Vesa";


![6-9](https://github.com/user-attachments/assets/fdb2ca1f-f8fb-4c46-b30e-871309730244)


Qno.10 ans

select name from airport where latitude_deg in (select min(latitude_deg) from airport);


![6-10](https://github.com/user-attachments/assets/5a67724e-cc23-4cee-860d-47be4beb6321)



