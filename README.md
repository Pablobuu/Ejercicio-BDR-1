# Ejercicio-BDR-1
Comandos SQL para ejercicio en PostgreSQL

SELECT * FROM clientes;

CREATE table clientes (email varchar(50),
					  nombre varchar,
					  telefono varchar(16),
					  empresa varchar(50),
					  prioridad smallint);

INSERT INTO clientes VALUES 
('pepegrillo@gmail.com', 'Pepe Grillo', '+25553698', 'Aplaplac', 10),
('jcbodoque@gmail.com', 'Juan Carlos Bodoque', '+25558844', 'Ecoplac', 9),
('spiderman@gmail.com', 'Peter Parker', '+25552216', 'Marvel', 10),
('mostroshrek@gmail.com', 'Shrek Ogro', '+25556633', 'Pantano S.A.', 8),
('pepepalotes@gmail.com', 'Pepito Palotes', '+25558132', 'Sodimac S.A.', 7);

SELECT * FROM clientes  MAX(prioridad) LIMIT 3;

SELECT * FROM clientes WHERE prioridad = 10;
