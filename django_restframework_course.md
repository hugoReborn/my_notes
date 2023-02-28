# Curso Django y  Django Rest framework.

- Django Rest framework es un framework de paython para el desarrollo web
- un framework es un marco de trabajo, en este caso un marco de trabajo para Python esto quiere decir que es una 
 manera para llevar a cabo desarrollos con el lenguaje Python.
Los frameworks automatizan una seria de procesos ahorrándonos una gran cantidad de líneas de código
Los frameworks nos brindan un patron de diseño, el cual seguiremos dependiendo del lenguaje que 
estemos utilizando

# Instalacion de Django `(Django 4)`

## `Entornos Virtuales (env - venv)` 
Los entornos virtuales son espacios de trabajo apartados de la memoria y almacenamiento
central de nuestro computador donde podemos realizar configuraciones e instalaciones sin afectar nuestro computador

Los entornos virtuales se utilizan principalmente para evitar conflictos entre versiones de un 
determinado paquete 

## `Creacion de un Ambiente Virtual `
````mermaid
flowchart LR
python --> -m
-m --> venv
venv --> nombre_entorno
lenguaje --> indicamos_tipo_paquete_python
indicamos_tipo_paquete_python --> entorno_virtual
entorno_virtual --> elegir_nombre

````

```
Con el script anterior ya tendriamos una carpeta creada en nuestro directorio nuestro entorno virtual
```
Para poder hacer uso de este entorno virtual que hemos creado debemos activarlo, en la terminal nos movemos hasta el directorio llamado 
`Scripts` y cuando nos encontremos dentro de este directorio ejecutamos el siguiente comando 
``./activate``

Esto nos devolverá en consola lo siguiente 

```
(nombre_entorno) C:\Users\Usuario\Documents\Proyectos\django_restframework_course\Scripts>
```

# Creacion de un proyecto Django en terminal
Antes de crear nuestro proyecto debemos fijarnos en el directorio en que nos encontremos,
ya que al crear el proyecto quedara dentro del directorio en que nos encontremos
creamos un proyecto con el siguiente comando 
```
django-admin startproject nombre_proyecto
```

Este comando nos creará una nueva carpeta en nuestro directorio donde vivira el proyecto django y sus
archivos principales
- manage.py
- init.py 
- settings.py
- urls.py
## Composicion de un Proyecto Django 
___
````mermaid
graph LR
A[proyecto django] -----> B[bases de datos]
A[proyecto django] -----> C[vistas]
A[proyecto django] -----> D[urls]
A[proyecto django] -----> E[aplicacion1]
A[proyecto django] -----> F[aplicacion2]
````

```
Cada Aplicacion debe dedicarse a una logica de negocio especifica y esta puede y debe ser reutilizada
Cada Aplicacion debe ser lo mas independiente posible de las demas aplicaciones
```

# Proyecto Empleados
| empleados                     | listar | departamentos | administrar |
|-------------------------------|--------|---------------|-------------|
| Imagen                        |
 | Sistema Registro de Empleados |

## Listar
Listar será una pestaña donde podremos listar los trabajadores ingresados en la base de datos 

## Departamentos