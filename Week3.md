# Database
week 3 exercise.
Qno.1
select * from goal;

![qno 1](https://github.com/user-attachments/assets/70940ea1-28d5-487c-9cbe-6bf416960aab)

Qno.2
select name, type from airport where iso_country = 'FI';

![qno 2](https://github.com/user-attachments/assets/d148aa22-4a87-4516-9d26-984884dadbc5)

Qno.3
select name from airport where iso_country = 'FI' order by name asc;


![qno 3 (2)](https://github.com/user-attachments/assets/610bd0bb-c763-41ee-b9fa-240ade217943)

Qno.4
select name,type from airport where iso_country = 'FI' order by type asc, name asc;
![qno 4 (2)](https://github.com/user-attachments/assets/27f89a15-72ec-4e06-a5ad-0771ba409ba8)

Qno.5
select name from country where name like 'F%';


![qno 5 (2)](https://github.com/user-attachments/assets/880e516c-f3ee-4eed-8954-96d99f27c826)

Qno.6
select name from country where name like "%F%";

![qno6](https://github.com/user-attachments/assets/f3ee0e3a-c529-405d-a03d-6b70d8c35d94)

Qno.7
select location from game where screen_name "%Vesa%";

![qno 7](https://github.com/user-attachments/assets/ff692076-e935-4aa2-8f62-c513f6be1d98)

Qno.8
select co2_consumed from game where screen_name = "Ilkka";

![qno 8](https://github.com/user-attachments/assets/e1ca9b63-33e0-4522-9fc2-38d1a0689683)

Qno.9
select distinct co2_budget from game;

![qno 9](https://github.com/user-attachments/assets/dd8bae6e-5b4d-4500-ad1b-e74f33dfc08e)

Qno.10
set @co2_left = 0;
select screen_name ,co2_budget, co2_consumed,(co2_budget - co2_consumed) as co2_left from game where screen_name = "Ilkka";

![qno 10](https://github.com/user-attachments/assets/1adbaf8a-22bd-4643-981f-2b495f30e7a6)


