Week 3 excercise 3:
Qno.1 ans
select country.name as "country name", airport.name as "airport name" from country, airport where country.iso_country and country.name = 'Iceland';


![3-1](https://github.com/user-attachments/assets/ee89620f-fe5c-49b9-8c81-f5b8a3ef3e50)


Qno.2 ans
select airport.name as "airport name" from airport join country on airport.iso_country= country.iso_country where country.name = "France" and airport.type = "large_airport";


![3-2](https://github.com/user-attachments/assets/869098b5-e28e-4292-a06c-5d599eae9e65)


Qno.3 ans
select country.name as "country name", airport.name as "airport_name" from country, airport where airport.iso_country = country.iso_country and country.continent = "AN";


![3-3](https://github.com/user-attachments/assets/28132103-45cc-4765-ae10-c147a7a71032)


Qno.4 ans
select elevation_ft from airport join game on airport.ident = game.location where screen_name = "Heini";


![3-4](https://github.com/user-attachments/assets/018d762f-d154-407f-87aa-1d7dbbc043f9)


Qno.5 ans
set @elevation_m = 0;
select (elevation_ft * 0.3048) as elevation_m from airport join game on airport.ident = game.location where screen_name = "Heini";


![3-5](https://github.com/user-attachments/assets/2b86161d-2da6-4fc7-be74-233e01089be4)


Qno.6 ans
select name from airport join game on airport.ident = game.location where screen_name = "Ilkka";


![3-6](https://github.com/user-attachments/assets/5f983013-c250-431f-a39c-455dd13e66c7)


Qno.7 ans
select country.name from country, airport, game where game.location = airport.ident and airport.iso_country = country.iso_country and game.screen_name = "Ilkka";


![3-7](https://github.com/user-attachments/assets/69d8b92b-462f-4758-af4a-bfc5c25bc7a7)


Qno.8 ans
select goal.name from goal, goal_reached, game where goal.id=goal_id and game.id= game_id and screen_name = "Heini";


![3-8](https://github.com/user-attachments/assets/f8262e16-a914-4c51-a71f-fe66c0f81585)


Qno.9 ans
select airport.name from airport, game, goal_reached, goal where airport.ident = game.location and game.id = game_id and goal.id = goal_id and game.screen_name = "Ilkka" and goal.name = "clouds";


![3-9](https://github.com/user-attachments/assets/565e2c91-da87-40ad-b282-b3e02d3de473)


Qno.10 ans
select country.name from airport, country, game, goal, goal_reached where country.iso_country = airport.iso_country and airport.ident = game.location and game.id = goal_reached.game_id and goal.id = goal_reached.goal_id and game.screen_name = "Illka" and goal.name = "clouds";


![3-10](https://github.com/user-attachments/assets/1a92ff0f-8e12-483d-86b1-4c2c5adec587)



