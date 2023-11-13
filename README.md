# gesifar-api

`npm start `

to visualize data in the browser

**in Lagaron:**

create database called gasifar-api
run following SQL commands:
```
CREATE TABLE `usuarios` (
	`id` INT NOT NULL AUTO_INCREMENT,
	`name` VARCHAR(50) NULL DEFAULT NULL,
	`lastname` VARCHAR(50) NULL DEFAULT NULL,
	`email` VARCHAR(50) NULL DEFAULT NULL,
	`password` VARCHAR(50) NULL DEFAULT NULL,
	`role` varchar(50) COLLATE utf8mb4_general_ci DEFAULT NULL,
	PRIMARY KEY (`id`)
)
COLLATE='utf8mb4_general_ci'
ENGINE=InnoDB
;

INSERT INTO usuarios(NAME,lastname,email,PASSWORD) VALUES('Laura','Schell','admin1@gmail.com','admin1');

INSERT INTO usuarios(NAME,lastname,email,PASSWORD) VALUES('Javier','Medina','admin2@gmail.com','admin2');

CREATE TABLE `profesionales` (
	`id` INT NOT NULL AUTO_INCREMENT,
	`dni` VARCHAR(10) NULL DEFAULT NULL,
	`name` VARCHAR(50) NULL DEFAULT NULL,
	`lastname` VARCHAR(50) NULL DEFAULT NULL,
	`profesion` VARCHAR(50) NULL DEFAULT NULL,
	`area` VARCHAR(50) NULL DEFAULT NULL,
	PRIMARY KEY (`id`)
)
COLLATE='utf8mb4_general_ci'
ENGINE=InnoDB
;

INSERT INTO profesionales(dni, NAME,lastname,profesion,area) VALUES('23456789','Maria','Lopez','Enfermera','Cirugia General');

INSERT INTO profesionales(dni, NAME,lastname,profesion,area) VALUES('54657698','Jose','Gomez','Medico','Pediatria');


CREATE TABLE IF NOT EXISTS `materiales` (
  `id` int NOT NULL AUTO_INCREMENT,
  `tipo` varchar(50) CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci DEFAULT NULL,
  `forma` varchar(50) CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci DEFAULT NULL,
  `presentacion` varchar(50) CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci DEFAULT NULL,
  `fecha_venc` date DEFAULT NULL,
  KEY `id` (`id`)
)

INSERT INTO materiales (id, tip, forma, presentacion, fecha_venc) VALUES
	(1, 'Insumo', 'FORMA 1', '33', '2024-05-29'),
	(2, 'Medicamento', 'forma2', 'pres2', '2024-11-19'),
	(3, 'Medicamento', 'FORMA 3', 'QWEWQE', '2023-10-14'),
	(4, 'Insumo', 'FORMA 4', 'ss', '2023-11-04');`
```
