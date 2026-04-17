# Propuesta TP DSW

## Grupo
### Integrantes
* 47141 - Santiago Jesus Fernandez

### Repositorios
* [PWA para clientes]([http://hyperlinkToGihubOrGitlab](https://github.com/S4ntifdz/Tp-Estacionamiento-PWA.git))
* [Backend con Server side rendering del dashboard para administradores]([http://hyperlinkToGihubOrGitlab](https://github.com/S4ntifdz/Estacionamiento-Core.git))

## Tema
### Descripción
Sistema de gestion de plazas de estacionamiento, admite reservas inmediatas o por adelantado, con un dashboard para el administrador del estacionamiento y una pwa para los clientes. La misma se maneja con saldo cargado en la cuenta del usuario.

### Modelo
<img width="1092" height="720" alt="image" src="https://github.com/user-attachments/assets/595ae62e-7d58-4f5a-ba03-cf6384523cdb" />

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Estacionamiento<br>2. CRUD Plazas de estacionamiento<br>3. CRUD Usuarios<br>3. CRUD Saldo|
|CRUD dependiente|1. CRUD Plazas de estacionamiento {depende de} CRUD Estacionamiento<br>2. CRUD Transaccion {depende de} Usuario |
|Listado<br>+<br>detalle| 1. Listado de habitaciones filtrado por tipo de habitación, muestra nro y tipo de habitación => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Estacionamiento<br>2. CRUD de Plazas de estacionamiento<br>3. CRUD Usuarios<br>4. CRUD Saldo<br>|
|CUU/Epic|1. Reservar una plaza de estacionamiento y que esta impacte en el dashboard de administracion en el dia de la fecha<br>2. Manejo de cierre de caja al final del dia<br>|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.
Social login con google
Modelo de negocio multitenant "row level"

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

