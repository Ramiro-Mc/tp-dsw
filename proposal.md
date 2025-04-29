# Propuesta TP DSW

## Grupo
### Integrantes
* 52992 - Martinez Castro, Ramiro Facundo
* 52838 - López, Joaquín
* 52959 - García Marianelli, Matías Fenando
* 53020 - Busnadiego, Martín
* 53400 - Spedaliere, Mateo

### Repositorios
* [fullstack app](https://github.com/Ramiro-Mc/dsw-fullstack-app)

## Tema

Página de cursos educativos online 

### Descripción

* El sistema permitirá a los usuarios ingresar a la pagina web, registrarse e inscribirse a los cursos disponibles, realizando pagos a través de una pasarela de pagos.

* Un usuario puede tambien dar de alta un curso de forma gratuita. El administrador despues de verificar el mismo, le informara al creador la comision que este tendra por cada venta. Tambien el creador puede pagar por publicidad de su curso para cierta cantidad de días.

* Por lo tanto, un usuario puede navegar por la pagina como cliente y dueño de un curso de forma simultanea.

* El creador de un curso tendra su propia interfaz para administrar o actualizar ciertas caracteristicas del mismo (contenido, precios, anuncios, etc.).

* Desde la vista de un usuario los cursos contaran con una interfaz especial en la cual se puede elegir la leccion a tomar (video y/o pdf) y llevar un registro del progreso del curso.

* Dentro de cada curso habrá una seccion llamada "comunidad" pensada para que los usuarios que estan realizando el mismo puedan intercambiar dudas/opiniones y dar feedback al creador del curso.

### Modelo
![Alt](https://github.com/Ramiro-Mc/tp-dsw/blob/main/Diagrama.png?raw=true)

## Alcance Funcional 

### Alcance Mínimo


Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Curso<br>2. CRUD Cliente <br> 3. CRUD Administrador <br> 4. CRUD TipoCurso |
|CRUD dependiente|1. CRUD Leccion {depende de} CRUD Curso
|Listado<br>+<br>detalle| 1. Listado de lecciones por curso, ordenado por número de lección => detalle muestra título de la lección, descripció y duración<br> 2. Listado de cursos filtrado por estado, duración, tipo de curso, costo y nombre del creador => detalle muestra titulo de curso, costo y duración|
|CUU/Epic|1. Inscribirse a un curso<br>2. Publicar un curso <br> 3. Tomar lecciones|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Curso<br>2. CRUD Cliente<br>3. CRUD Administrador<br>4. CRUD TipoCurso<br>5. CRUD Comunidad <br>6. CRUD Publicacion <br>7. CRUD Descuento|
|CUU/Epic|1. Dar de baja un curso<br>2. Mostrar facturación generada con cada curso<br>3. Aplicar descuento a curso <br> 4. Dar una puntuacion a un curso


### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Listados |1. Listado de cursos adquiridos<br>2. Listado de cursos en promocion<br>3. Listado de cursos creados|
|CUU/Epic|1. Contratar publicidad para un curso<br>|
|Otros|1. Envío de notificaciones de comunidad a email <br>2. Envio de notificaciones sobre vencimiento de membresia al mail<br>3. Envio de notificaciones sobre promociones de cursos|


