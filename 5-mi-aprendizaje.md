# Reflexión sobre los aprendizajes

Comparando mis conocimientos antes de hacer la práctica con los adquiridos después de realizar la tarea, puedo destacar los siguientes aprendizajes principales para mi formación profesional:

- Antes de la práctica, ya conocía la funcionalidad básica de los comandos de Docker para crear contenedores y manejar variables de entorno. Gracias a esto, pude configurar correctamente las variables de entorno del contenedor de MySQL, asignando una contraseña al usuario root y utilizando un archivo .env dentro de la hipervisualizadora.

- Durante la práctica, aprendí a simplificar y optimizar comandos para cumplir la misma función de manera más eficiente, lo que mejora la productividad al trabajar con contenedores.

- Profundicé en la gestión de datos confidenciales, descubriendo cómo Docker permite proteger información sensible mediante **Docker Secrets**. Esto asegura que contraseñas, claves API y certificados se almacenen cifrados y solo sean accesibles por los contenedores autorizados, evitando exposición accidental en imágenes o archivos de configuración.

# Docker Secrets

Docker Secrets es una funcionalidad diseñada para manejar información sensible de forma segura en contenedores, especialmente útil en entornos de producción y clústeres.

### Características

- **Acceso controlado:** solo los contenedores que lo necesitan pueden leer el secreto.  
- **Transporte seguro:** los secretos se transmiten cifrados a los nodos del clúster.  
- **Ciclo de vida limitado:** los secretos se eliminan automáticamente cuando el servicio se detiene o se actualiza.  
- **Integración con Swarm:** facilita la gestión centralizada de credenciales en clústeres Docker Swarm.

