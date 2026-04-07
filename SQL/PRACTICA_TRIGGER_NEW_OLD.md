Extensión Áulica “DRAGO”

Carrera: Técnico Superior en Desarrollo de Software
Cátedra: Base de Datos II- 2019 (3er año)
Docente: Cortés María Fernanda

TRIGGERS: USO DE CLÁUSULAS NEW, OLD EN DISTINTOS MOMENTOS
Crear las siguientes tablas:
CREATE TABLE `libros` (
  `IdLibro` int(11) NOT NULL primary key auto_increment,
  `AutorId` int(11) NOT NULL,
  `GeneroId` int(11) NOT NULL,
  `Titulo` varchar(200) NOT NULL,
  `Disponible` tinyint(1) NOT NULL,
  `fecha_prestamo` date DEFAULT NULL
) 
Ingresar los siguientes valores en la tabla libros:
 (‘’, 1, 2, 'Rayuela', 1, NULL),
(‘’, 3, 2, 'Cien años de soledad', 0, NULL),
(‘’, 2, 1, 'El hacedor', 0, '2019-08-14');
CREATE TABLE `prestamos` (
  `IdPrestamo` int(11) NOT NULL primary key auto_increment,
  `SocioDni` int(11) NOT NULL,
  `LibroId` int(11) NOT NULL,
  `FechaPrestamo` date NOT NULL,
  `FechaDevolucion` date DEFAULT NULL
);
Ingresar los siguientes valores en la tabla préstamos:
(‘ ’, 11111111, 2, '2019-08-10', NULL),
(‘ ’, 11111111, 3, '2019-08-24', NULL),
( ‘ ’, 11111111, 3, '2019-08-14', NULL);

Ejercicios:
1-	Guardar los datos de la  tabla préstamos que se eliminan en una tabla llamada historial_prestamo, crear la tabla primero.

2-	Al momento de ingresar un préstamo, se deberá actualizar automáticamente Crear un trigger que al ingresar en la tabla libros la disponibilidad: 1- disponible, 0 no disponible y registre en el campo fecha_prestamo, la fecha en la que realizo el préstamo

3-	Con el trigger anterior se logró una consulta que el sistema automáticamente modificara el estado de la tabla Libros a No Disponible y se registró la fecha del préstamo. Al momento que el socio realiza la devolución y hay que volver a modificar el estado de la tabla Libros, con que herramienta realizaría esta operación?


