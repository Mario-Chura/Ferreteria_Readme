<div align="center">
<table>
    <theader>
        <tr>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/epis.png?raw=true" alt="EPIS" style="width:50%; height:auto"/></td>
            <th>
                <span style="font-weight:bold;">UNIVERSIDAD NACIONAL DE SAN AGUSTIN</span><br />
                <span style="font-weight:bold;">FACULTAD DE INGENIERÍA DE PRODUCCIÓN Y SERVICIOS</span><br />
                <span style="font-weight:bold;">ESCUELA PROFESIONAL DE INGENIERÍA DE SISTEMAS</span>
            </th>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/abet.png?raw=true" alt="ABET" style="width:50%; height:auto"/></td>
        </tr>
    </theader>
    <tbody>
        <tr><td colspan="3"><span style="font-weight:bold;">Formato</span>: Guía de Práctica de Laboratorio / Talleres / Centros de Simulación</td></tr>
        <tr><td><span style="font-weight:bold;">Aprobación</span>:  2022/03/01</td><td><span style="font-weight:bold;">Código</span>: GUIA-PRLE-001</td><td><span style="font-weight:bold;">Página</span>: 1</td></tr>
    </tbody>
</table>
</div>

<div align="center">
<span style="font-weight:bold;">INFORME DE LABORATORIO</span><br />

<table>
<theader>
<tr><th colspan="6">INFORMACIÓN BÁSICA</th></tr>
</theader>
<tbody>
<tr><td>ASIGNATURA:</td><td colspan="5">Progamación Web 2</td></tr>
<tr><td>TÍTULO DE LA PRÁCTICA:</td><td colspan="5">Proyecto Web - Ferreteria Online</td></tr>
<tr>
<td>NÚMERO DE PRÁCTICA:</td><td>08</td><td>AÑO LECTIVO:</td><td>2022 A</td><td>NRO. SEMESTRE:</td><td>III</td>
</tr>
<tr>
<td>FECHA DE PRESENTACIÓN:</td><td>23/08/2022</td><td>HORA DE PRESENTACIÓN: 12:00 pm</td><td colspan="3"></td>
</tr>
<tr><td colspan="3">INTEGRANTE(s):
<ul>
      <li><a href="https://github.com/Daunsa">Daniel Edwad Tapia Saenz</a></li>
			<li><a href="https://github.com/timysuclle3">Michael Benjamin Suclle Suca</a></li>
			<li><a href="https://github.com/Jerbo03">José André Paredes Quispe</a></li>
			<li><a href="https://github.com/Icielo23">Valery Cielo Iquise Mamani</a></li>
			<li><a href="https://github.com/Mario-Chura">Mario Franco Chura Puma</a></li>
</ul>
</td>
<td>NOTA:</td><td colspan="2"></td>
</<tr>
<tr><td colspan="6">DOCENTE(s):
<ul>
<li>Richart Smith Escobedo Quispe - rescobedoq@unsa.edu.pe</li>
</ul>
</td>
</<tr>
</tbody>
</table>
</div>

#   WebApp con Django

[![License][license]][license-file]
[![Downloads][downloads]][releases]
[![Last Commit][last-commit]][releases]

[![Debian][Debian]][debian-site]
[![Git][Git]][git-site]
[![GitHub][GitHub]][github-site]
[![Vim][Vim]][vim-site]
[![Java][Java]][java-site]

##  ***___1. Tipo de Sistema___***

Se trata de una aplicación web construida con el framework Django 4, que permita la inscripción de los alumnos en los horarios de laboratorios establecidos cada inicio de semestre.

##  Requisitos del sistema
   El sistema debe satisfacer los siguientes requisitos funcionales y no funcionales:

   - RQ01 : El sistema debe estar disponible en Internet a traves de una URL.
   - RQ02 : El sistema debe permitir el inicio/cierre de sesión.
   - RQ03 : El sistema debe permitir gestionar el año académico, cursos, profesores y las asignaciones de carga académica.
   - RQ1: La aplicación web permitirá al usuario iniciar sesión con su cuenta de google.
   - RQ2: La aplicación web emitirá un correo electrónico cuando se creen cuentas para validar el email.
   - RQ3: La aplicación web deberá generar en pdf el pedido realizado enviando una copia al emisor y receptor de la operación.
   - RQ4: La aplicación web tendrá un carrito de compras para todos los productos que el cliente desee comprar. 
   - RQ5: La aplicación web tendrá un apartado de pedidos a domicilio para materiales de construcción que se requieran en obra.
   - RQ6: La aplicación podría generar códigos de barras. 
   - RQ7: Se establecerá contacto con los proveedores desde la página web.
   - RQ8: La aplicación web contará con un código de verificación para verificar el envío exitoso de su pedido.
   - RQ9: Se podrá anular la compra después de los primeros 15 min de confirmar.
   - RQ10: Promociones y descuentos a los usuarios serán notificadas por email.
   - RQ11: Las acciones realizadas por día como la actualización de inventario, serán notificadas y resumidas vía email.
   - RQ12: Habrá una categoría para usuarios Premium que tendrán beneficios de descuentos y accesos a artículos reservados “Premium” 
   - RQ13: La aplicación podrá modificar, eliminar, crear y leer datos con facilidad.
   - RQ14: La aplicación web contará con una base de datos correspondiente para generar ventas, almacenaje y usuarios.
   - RQ15: Tendrá la opción de un chat bot o un asistente en vivo para hacer consultas en la misma página y también tendrá una opción para redirigir a un chat de WhatsApp.
   - RQ16: La aplicación web tendrá un apartado de soporte para reportar reclamos, sugerencias, o para solicitar alguna recomendación, ante los productos.
   - RQ17: En el carrito de compras se permitirá comparar productos, y sus atributos como peso, precio, descuentos, ventajas y precauciones.
   - RQ18: Los productos tendrán categorías para facilitar la compra de los clientes.
   - RQ19: Se incluirá un buscador de productos.
   - RQ20: La aplicación web tendrá un diseño responsivo para que se pueda adaptar a pantallas de diferentes tamaños con un solo sitio web.

   

##  ***___2. Modelo de datos___***
   El modelo de datos esta conformado por las siguientes entidades.

   -   Curso : En esta entidad se almacena la información de los cursos o asignaturas que se imparten en una Escuela Profesional. Ejemplo: Programación Web 2, III semestre, 02 horas teóricas, 04 horas de laboratorio, etc..
   -   Profesor : En esta entidad se almacena los datos de los profesores que se responsabilizan del avance académico en la enseñanza de los temas planificados en cada curso. Ejemplo: Richart Escobedo, rescobedoq@unsa.edu.pe, Magister, etc.

    ...

##  Diccionario de datos

   Se implementaron los siguientes modelos con sus respectivos atributos:

| tienda_producto | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| nombre  | varchar(50)|  "nombre" varchar(50) NOT NULL | 
| imagen  | varchar(100)| "imagen" varchar(100) NOT NULL | 
| precio  | real| "precio" real NOT NULL | 
| disponibilidad  | bool| "disponibilidad" bool NOT NULL | 
| created  | date| "created" date NOT NULL | 
| updated | date| "updated" date NOT NULL | 
| categorias_id  | bigint| "categorias_id" bigint NOT NULL |

| tienda_categoriaprod | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| nombre  | varchar(50)|  "nombre" varchar(50) NOT NULL |  
| created  | date| "created" date NOT NULL | 
| updated | date| "updated" date NOT NULL | 

| lineapedidos | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| cantidad  | integer|  "cantidad" integer NOT NULL | 
| created_at  | datetime| "created_at" datetime NOT NULL | 
| pedido_id  | bigint| "pedido_id" bigint NOT NULL | 
| producto id | bigint| "producto_id" bigint NOT NULL | 
| user_id  |Integer | "user_id" integer NOT NULL | 

| pedidos | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| created_at  | datetime| "created_at" datetime NOT NULL | 
| user_id  |Integer | "user_id" integer NOT NULL | 

| servicios_servicio | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| titulo  | varchar(50)|  "titulo" varchar(50) NOT NULL | 
| imagen  | varchar(100)| "imagen" varchar(100) NOT NULL | 
| created  | datetime| "created" datetime NOT NULL | 
| updated | datetime| "updated" date NOT NULL | 
| contenido  | varchar(1000)| "contenido" varchar(1000) NOT NULL | 

| ferreteriaOnlineApp_producto | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| nombre  | varchar(200)|  "nombre" varchar(200) NOT NULL | 
| marca  | varchar(200)|  "marca" varchar(200) NOT NULL | 
| precio  | decimal | "precio" decimal NOT NULL | 
| stock  | integer| "stock" integer NOT NULL | 
| reservado | bool| "reservado" bool NOT NULL |
| descontable | real| "precio" real NOT NULL | 
| fecha_publicacion  | datetime| "fecha_publicacion" datetime NOT NULL | 
| imagen  | varchar(100)| "imagen" varchar(100) | 
| categorias_id  | bigint| "categorias_id" bigint NOT NULL |

| ferreteriaOnlineApp_categoria | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| nombre  | varchar(200)|  "nombre" varchar(200) NOT NULL |  
| fecha_publicacion  | date| "fecha_publicacion" date NOT NULL | 

| blog_post | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| titulo  | varchar(500)|  "titulo" varchar(50) NOT NULL | 
| imagen  | varchar(100)| "imagen" varchar(100) |
| created  | datetime| "created" datetime NOT NULL | 
| updated | datetime| "updated" datetime NOT NULL | 
| autor_id | integer| "autor_id" integer NOT NULL |
| contenido  | varchar(1000)| "contenido" varchar(1000) NOT NULL |

| blog_categoria | | |
| -- | -- | -- |
| Name  | Type  | Schema | 
| id  | integer  | "id" integer NOT NULL | 
| nombre  | varchar(50)|  "nombre" varchar(50) NOT NULL | 
| created  | datetime| "created" datetime NOT NULL | 
| updated | datetime| "updated" datetime NOT NULL | 


##  Diagrama Entidad-Relación
    ...

##  ***___3. Administración con Django___***
   Se muestran los pasos realizados para crear el Proyecto, la aplicación, creacion de modelos, migraciones y habilitación del panel de administración en Django.
    ...

##  ***___4. Plantillas Bootstrap___***
   Se seleccionó la siguiente plantilla para el usuario final (No administrador).

   Demo online:
    URL: https://www.free-css.com/free-css-templates/page246/freshshop

   Se muestran las actividades realizadas para adecuación de plantillas, vistas, formularios en Django.
    ...

##  ***___5. CRUD - Core Business - Clientes finales___***
   El núcleo de negocio del sistema de inscripciones tiene valor de aceptación para los cliente finales (alumnos) radica en realizar el proceso de inscripción propiamente, que empieza desde que:
    1. El alumno inicia sesión.
    2. El alumno selecciona el o los cursos donde desea realizar una inscripción.
    3. El alumno selecciona el grupo de laboatorio donde desea incribirse.
    4. El alumno puede tener la posibilidad de anular una incripción por varias razones: cambio de grupo, corregir error, etc.
    5. El alumno puede ver el consolidado de sus inscripciones.
    6. El alumno cierra sesión.

   Todas y cada una de estas pantallas debe funcionar en la plantilla bootstrap.
    A continuación se muestran las actividades realizadas para su construcción:
    ...

##  ***___6. Servicios mediante una API RESTful___***
   Se ha creado una aplicación que pondra a disposición cierta información para ser consumida por otros clientes HTTP.
    1. GET : Con el método get se devolverá la lista de cursos, grupos y horarios establecidos para que el alumno sobre todo vea esta información en cualquier otro medio. En formato JSON. 
    2. POST : Con este método se enviara el código del alumno y se devolvera sus inscripciones. En formato JSON.
    
   Ejemplo: Prueba en Página web, aplicación móvil, PDF, etc.
    Se especifican los pasos para crear el servicio RestFul
    ...

##  ***___7. Operaciones asíncronas AJAX___***
   Se propone el uso de AJAX para realizar la asignación de carga académica a los docentes que estan registrados. Esta operación la realizará el usuario operador encargado por el DAISI.
   Se muestran los pasos necesarios a realizar.
    ....

## ***___8. Investigación:___***
   - Email: Se utilizará la funcionalidad del uso de envío de correos electrónicos cuando el proceso de inscripciones culmine y al profesor le llegue la lista de alumnos inscritos en sus grupos a cargo.
   - Upload: Se utilizará esta funcionalidad para subír, archivos CSV para importar y exportar información en el sistema.
    Se muestran los pasos realizados para su funcionamiento correcto.
    ...

Github del proyecto:

URL en Heroku:https://ferreteriamisti.herokuapp.com/

URL Playlist YouTube: https://youtube.com/playlist?list=PLY9ZwtuLx1XO4YZvTq0LFWy8ehwF46HL-
El PlayList en YouTube está formado por la explicación de los siguientes requerimientos:
- Video 01 - Tipo de sistema y Requisitos. URL: 
- Video 02 - Modelo de datos - DD - DER. URL: 
- Video 03 - Administración con Django. URL:
- Video 04 - Plantillas Bootstrap. URL:
- Video 05 - CRUD. URL:
- Video 06 - Servicios REST.
- Video 07 - Realizar Operaciones asíncronas AJAX. URL:
- Video 08 - Investigación: Uso de el componente de Email. URL:



## REFERENCIAS
-   https://www.free-css.com/free-css-templates/page246/freshshop
-   https://docs.djangoproject.com/en/4.0/intro/tutorial06/
-   https://www.youtube.com/watch?v=iQN0z6MDrEY&ab_channel=pildorasinformaticas
-   https://developer.mozilla.org/es/docs/Learn/Server-side/Django/Home_page

#

[license]: https://img.shields.io/github/license/rescobedoq/pw2?label=rescobedoq
[license-file]: https://github.com/rescobedoq/pw2/blob/main/LICENSE

[downloads]: https://img.shields.io/github/downloads/rescobedoq/pw2/total?label=Downloads
[releases]: https://github.com/rescobedoq/pw2/releases/

[last-commit]: https://img.shields.io/github/last-commit/rescobedoq/pw2?label=Last%20Commit

[Debian]: https://img.shields.io/badge/Debian-D70A53?style=for-the-badge&logo=debian&logoColor=white
[debian-site]: https://www.debian.org/index.es.html

[Git]: https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white
[git-site]: https://git-scm.com/

[GitHub]: https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white
[github-site]: https://github.com/

[Vim]: https://img.shields.io/badge/VIM-%2311AB00.svg?style=for-the-badge&logo=vim&logoColor=white
[vim-site]: https://www.vim.org/

[Java]: https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white
[java-site]: https://docs.oracle.com/javase/tutorial/


[![Debian][Debian]][debian-site]
[![Git][Git]][git-site]
[![GitHub][GitHub]][github-site]
[![Vim][Vim]][vim-site]
[![Java][Java]][java-site]


[![License][license]][license-file]
[![Downloads][downloads]][releases]
[![Last Commit][last-commit]][releases]
