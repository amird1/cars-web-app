# cars-web-app
Web app coded in java for ordering a vehicle
Database created using MySQL containing few car makes, model, color and price. 3 tables (cars, ModelColors, prices) in the schema of the database.


Database MySQL code as follows:



CREATE DATABASE carsback;

USE carsback;
CREATE table cars
(
Make varchar (30)
);


INSERT INTO cars (Make) values ('Honda');
INSERT INTO cars (Make) values ('Toyota');
INSERT INTO cars (Make) values ('Nissan');


---------------------next code set is on separate query tab on MySQL Workbench------------------------------------------------------


USE carsback;

CREATE table ModelColors
(
ID int NOT NULL AUTO_INCREMENT, Make varchar (30), Model varchar (30) , color varchar (20),
primary key (ID)
);

INSERT INTO ModelColors (Make, Model, color) values ('Honda', 'Civic', 'white');
INSERT INTO ModelColors (Make, Model, color) values ('Honda', 'Civic', 'red');
INSERT INTO ModelColors (Make, Model, color) values ('Honda', 'Civic', 'black');

INSERT INTO ModelColors (Make, Model, color) values ('Toyota', 'Camry', 'white');
INSERT INTO ModelColors (Make, Model, color) values ('Toyota', 'Camry', 'red');
INSERT INTO ModelColors (Make, Model, color) values ('Toyota', 'Camry', 'black');

INSERT INTO ModelColors (Make, Model, color) values ('Nissan', 'Maxima', 'white');
INSERT INTO ModelColors (Make, Model, color) values ('Nissan', 'Maxima', 'red');
INSERT INTO ModelColors (Make, Model, color) values ('Nissan', 'Maxima', 'black');



---------------------next code set is on separate query tab on MySQL Workbench------------------------------------------------------


USE carsback;

CREATE TABLE prices
(
ID int NOT NULL AUTO_INCREMENT, Price int, Make varchar (30), Model varchar (30) , color varchar (20),
primary key (ID)
);

INSERT INTO prices (Price, Make, Model, color) values ('12000', 'Honda', 'Civic', 'white');
INSERT INTO prices (Price, Make, Model, color) values ('11000', 'Honda', 'Civic', 'red');
INSERT INTO prices (Price, Make, Model, color) values ('10000', 'Honda', 'Civic', 'black');

INSERT INTO prices (Price, Make, Model, color) values ('12000', 'Toyota', 'Camry', 'white');
INSERT INTO prices (Price, Make, Model, color) values ('11000', 'Toyota', 'Camry', 'red');
INSERT INTO prices (Price, Make, Model, color) values ('10000', 'Toyota', 'Camry', 'black');

INSERT INTO prices (Price, Make, Model, color) values ('12000', 'Nissan', 'Maxima', 'white');
INSERT INTO prices (Price, Make, Model, color) values ('11000', 'Nissan', 'Maxima', 'red');
INSERT INTO prices (Price, Make, Model, color) values ('10000', 'Nissan', 'Maxima', 'black');




----------------------------------------END----------------------------------------------------
