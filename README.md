## Ansible ejercicios varios (incluido 1 con roles) y despliegue-total
# En este reposito estan las practicas con Ansible y el despligue total con:
1. crear en gitlab el repositorio donde albergaremos y de donde recogeremos el artifacto
2. Generamos la llave privada y publica para el usuario app2
3. Aprovisionamiento con Ansible
   - Creación-Configuracion de usuario
   - Aprovisionamiento de las carpetas y ficheros necesarios
   - Configuracion de los ficheros necesarios para el posterior despliegue con Jenkins
4. Despliegue con Jenkins mediante las etapas de:
   - Configuración de la llave privada para que jenkins conectarse por ssh a la maquina remota y recoja la imagen y lance la APP
   - Recogida del Código y Aplicativo desde Repositorio Git
   - Realización de pruebas con JaCoCo, test y Pitest de Gradle
   - Prueba de analisis con Sonarqube
   - Contrucción de la App y de la imagen donde se despleguará la App
   - Tagueado con las diferentes etiquetas que necesitemos, nº construccion, latest, dev, etc y subida al Registry inseguro de Gitab
   - Test de Seguridad de imagen con Trivy
   - Despligue final de la App contenida en la imagen archivada anteriormente en el host remoto utilizando ssh