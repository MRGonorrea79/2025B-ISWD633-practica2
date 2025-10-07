# Variables de Entorno
### ¿Qué son las variables de entorno?
# COMPLETAR
Las variables de entorno son valores dinámicos que se utilizan para configurar el comportamiento de procesos y aplicaciones en un sistema operativo o contenedor.
En Docker, se usan para pasar configuraciones al contenedor sin modificar la imagen base, como usuarios, contraseñas, puertos o rutas.
### Para crear un contenedor con variables de entorno

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.

# COMPLETAR
docker run -d --name srv-nginx -e username=javier -e role=admin nginx:alpine

# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR
<img width="1871" height="641" alt="image" src="https://github.com/user-attachments/assets/a230b091-c92b-4620-b065-b5295c4c51cf" />

### Crear un contenedor con la imagen de mysql, mapear todos los puertos
# COMPLETAR
docker run -d --name srv-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123456 mysql

### ¿El contenedor se está ejecutando?
# COMPLETAR
<img width="1907" height="125" alt="image" src="https://github.com/user-attachments/assets/d10fe0a4-ca55-4fc4-91c1-d7209df0648c" />

### Identificar el problema
# COMPLETAR
En mi caso no existe ningun problema a presentar

### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

### Crear un contenedor con mysql, mapear todos los puertos y configurar las variables de entorno mediante un archivo
# COMPLETAR
docker run -d --name srv-mysql-env --env-file mysql.env -p 3306:3306 mysql
# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR 
<img width="1896" height="111" alt="image" src="https://github.com/user-attachments/assets/dd13ba42-424d-4f0d-a875-0bc37d8aaed1" />
<img width="1917" height="363" alt="image" src="https://github.com/user-attachments/assets/22996c53-e417-49f2-96c2-e33ca73e31db" />

### ¿Qué bases de datos existen en el contenedor creado?
# COMPLETAR
estan las propias de MYSQL y la propia llamada javier
<img width="965" height="219" alt="image" src="https://github.com/user-attachments/assets/00c723ff-c360-4087-809e-158c9250dd17" />
