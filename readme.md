###Proceso de despliegue

1) Plugin de jib  id 'com.google.cloud.tools.jib' version '2.2.0'

2) skaffold build. Construimos artefacto

3) k8s-deployment y service (creación de plantillas y añadimos al manifiesto de skaffold.yml)

3) skaffold run. Lanza el pipeline que hemos indicado en skaffold.

4) minikube service skaffold. Usando minikube obtenemos url de despliegue.

5) accedemos al estado del Actuator/actuator/health.

6) `skaffold dev` -> livereload

7) skaffold delete. Nos fundimos el service / deployment que hemos creado.
