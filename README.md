# Criando imagem

```
cd ./src

docker build -t kubedev/api-conversao-temperatura:v1 .
```

# Criando container

```
docker container run -d --name api -p 8080:8080 kubedev/api-conversao-temperatura:v1
```
