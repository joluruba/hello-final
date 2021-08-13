# Ejercicio Final de Curso con un despliegue total de ejemplo
## En este reposito esta el ejercicio de final de curso sobre un despligue total de una App donde se han seguido los siguientes pasos:
1. crear en gitlab el repositorio donde albergaremos y de donde recogeremos el artifacto
2. Generamos la llave privada y publica para el usuario app2
3. Aprovisionamiento con Ansible
   - Playbook ejecutado con  -K para facilitar la pass de root y poder subir dicho playbook para revision por profesor
   - Creación-Configuracion de usuario
   - Aprovisionamiento de las carpetas y ficheros necesarios
   - Configuracion de los ficheros necesarios para el posterior despliegue con Jenkins
4. Despliegue con Jenkins mediante las etapas de:
   - Configuración de la llave privada para que jenkins conectarse por ssh a la maquina remota y recoja la imagen y lance la APP
   - Recogida del Código y Aplicativo desde Repositorio Git
   - Realización de pruebas con JaCoCo, test y Pitest de Gradle
   - Prueba de analisis con Sonarqube
   - Contrucción de la App y de la imagen donde se desplegará la App
   - Tagueado con las diferentes etiquetas que necesitemos, nº construccion, latest, dev, etc y subida al Registry inseguro de Gitab
   - Test de Seguridad de imagen con Trivy
   - Despligue final de la App contenida en la imagen archivada anteriormente en el host remoto utilizando ssh