## Esquema para el ejercicio
![Imagen](esquema-4-ejercicio.PNG)

### Crear la red
# COMPLETAR

### Crear el contenedor mysql a partir de la imagen mysql:8, configurar las variables de entorno necesarias
# COMPLETAR

### Crear el contenedor wordpress a partir de la imagen: wordpress, configurar las variables de entorno necesarias
# COMPLETAR
<img width="1459" height="192" alt="image" src="https://github.com/user-attachments/assets/8009a26d-cad0-4509-948f-e29183ee8471" />

De acuerdo con el trabajo realizado, en el esquema del ejercicio el puerto a es 9300

Ingresar desde el navegador al wordpress y finalizar la configuración de instalación.
# COLOCAR UNA CAPTURA DE LA CONFIGURACIÓN
<img width="614" height="709" alt="image" src="https://github.com/user-attachments/assets/8cce435a-ec00-47c2-8f91-f3d11305be85" />

Desde el panel de admin: cambiar el tema y crear una nueva publicación.
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress
# COLOCAR UNA CAPTURA DEL SITO EN DONDE SEA VISIBLE LA PUBLICACIÓN.
<img width="866" height="757" alt="image" src="https://github.com/user-attachments/assets/491eb8e1-b1b6-47e3-b98f-0b50ea85db16" />

### Eliminar el contenedor wordpress
# COMPLETAR
<img width="1453" height="160" alt="image" src="https://github.com/user-attachments/assets/91d78c60-a535-4286-ae3d-5ecfaba74897" />

### Crear nuevamente el contenedor wordpress
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress
<img width="921" height="903" alt="image" src="https://github.com/user-attachments/assets/346ad1df-5c7a-4f55-841b-0b2bf29e9d6d" />

### ¿Qué ha sucedido, qué puede observar?
# COMPLETAR
Los datos publicaciones y la pagina en general se mantuvieron intactos gracias a que la informacion se guardaba en la base de datos mySQL y no en el contenedor de wordpress

