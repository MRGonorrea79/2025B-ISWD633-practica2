### Crear contenedor de Postgres sin que exponga los puertos. Usar la imagen: postgres:15-alpine3.21
# COMPLETAR
docker run -d --name srv-postgres -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=admin123 -e POSTGRES_DB=postgres postgres:15-alpine3.21

### Crear un cliente de postgres. Usar la imagen: dpage/pgadmin4

# COMPLETAR
docker run -d --name cliente-pgadmin -e PGADMIN_DEFAULT_EMAIL=admin@admin.com -e PGADMIN_DEFAULT_PASSWORD=1234 -p 5050:80 --link srv-postgres:postgres dpage/pgadmin4
La figura presenta el esquema creado en donde los puertos son:
- a: 5432
- b: 80
- c: 5050

![Imagen](esquema-2-ejercicio.PNG)

## Desde el cliente
### Acceder desde el cliente al servidor postgres creado.
# COMPLETAR CON UNA CAPTURA DEL LOGIN
<img width="1911" height="918" alt="image" src="https://github.com/user-attachments/assets/2daba2ba-7b9f-4b03-945f-b2ba77030645" />

### Crear la base de datos info, y dentro de esa base la tabla personas, con id (serial) y nombre (varchar), agregar un par de registros en la tabla, obligatorio incluir su nombre.
<img width="947" height="879" alt="image" src="https://github.com/user-attachments/assets/cebacd91-1a6e-42c7-a94c-927654589bf5" />

## Desde el servidor postgresl
### Acceder al servidor
### Conectarse a la base de datos info
# COMPLETAR
<img width="684" height="217" alt="image" src="https://github.com/user-attachments/assets/8ab7319f-ce63-42da-a60e-889698bf9708" />

### Realizar un select *from personas
# AGREGAR UNA CAPTURA DE PANTALLA DEL RESULTADO

<img width="209" height="87" alt="image" src="https://github.com/user-attachments/assets/dd728437-767a-4b42-866c-deec03c5c865" />

