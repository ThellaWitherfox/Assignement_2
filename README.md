# Assignement_2
sqlkod:

//create table

CREATE TABLE `sqlandjava`.`cars`(
`car_id` INT(11) NOT NULL,
`brand`VARCHAR(45) NOT NULL,
`color`VARCHAR(45) NOT NULL,
PRIMARY KEY (`car_id`));

//create rows and store theme with information

INSERT INTO `sqlandjava`.`cars`(`car_id`, `brand`, `color`) VALUES ('1', 'Volvo', 'Black');
INSERT INTO `sqlandjava`.`cars`(`car_id`, `brand`, `color`) VALUES ('2', 'Saab',  'Blue');
INSERT INTO `sqlandjava`.`cars`(`car_id`, `brand`, `color`) VALUES ('3', 'Audi', 'Red');
INSERT INTO `sqlandjava`.`cars`(`car_id`, `brand`, `color`) VALUES ('4', 'Ford', 'Green');

//create user and set access (to database)

CREATE USER user@localhost IDENTIFIED BY 'username';

GRANT SELECT ON sqlandjava.cars TO user@localhost;


