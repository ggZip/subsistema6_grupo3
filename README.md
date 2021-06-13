## Requirements
Python 3.5.2+

## Usage
To run the server, please execute the following from the root directory:

```
pip install -r requirements.txt
python -m swagger_server
```

and, for instance, open your browser to here:

```
http://localhost:8080/api/v1/recambios
```


## Running with Docker

To run the server on a Docker container, please execute the following from the root directory:

```bash
# building the image
docker build -t swagger_server .

# starting up a container
docker run -p 8080:8080 swagger_server
```

## Docker image

```
docker pull clatange/aos:latest
```

## Docker compose
```
El docker-compose se ha hecho a partir de las imagenes de los subsistemas por lo que solo hace falta el .yaml para su ejecución

Para lanzar el docker-compose se necesitará estar en el directorio donde se encuentra el archivo docker-compose.yaml y ejecutar el siguiente comando: 

docker-compose up
```

## Kubernetes
```
Iniciar minikube, estar en el directorio donde se encuentra el archivo kubernets.yaml y ejecutar el siguiente comando:

kubectl apply -f kubernets.yaml
```
