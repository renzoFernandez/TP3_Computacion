# TP3_Computacion
1)Borrar en caso de que exista un contenedor con el nombre "dynamodb" docker rm dynamodb

2)Crear red local docker network create awslocal

3)Correr contenedor dynamodb en puerto 8000 docker run -p 8000:8000 --network awslocal --name dynamodb amazon/dynamodb-local:1.16.0 -jar DynamoDBLocal.jar -sharedDb

4)Abrir shell en explorador localhost:8000/shell

5)Copiar y pegar el contenido de Creacion de tabla.txt, en el shell y correr el script

6)Levantar sam sam local start-api --docker-network awslocal
