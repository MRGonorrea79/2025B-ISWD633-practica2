# COMPLETAR  
Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  
Ya sabia de antemano la funcionalidad de estos comandos, razon por la que pude solucionar el problema al crear las variables de entorno asociadas al contenedor de mySQL,asociando una contraseña al usurio "root"

Consultar: Cómo se gestionan datos confidenciales con los secretos de Docker (Docker Secrets).
# Docker Secrets
Docker Secrets es una funcionalidad de Docker diseñada para manejar información sensible de forma segura, como contraseñas, claves API o certificados. Los secretos se almacenan cifrados en el gestor de Docker y solo los servicios autorizados pueden acceder a ellos durante la ejecución. Esto evita que datos confidenciales queden expuestos en imágenes, archivos de configuración o variables de entorno.

### Caracteristicas

- Acceso controlado: solo los contenedores que lo necesitan pueden leer el secreto.

- Transporte seguro: los secretos se transmiten cifrados a los nodos del clúster.

- Ciclo de vida limitado: los secretos se eliminan automáticamente cuando el servicio se detiene o se actualiza.

- Integración con Swarm: Docker Secrets funciona de forma nativa en entornos Docker Swarm, facilitando la gestión centralizada de credenciales en clústeres.
