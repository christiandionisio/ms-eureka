# Módulo: ms-eureka
Para ejecutar localmente, se necesita ejecutar los siguientes comandos


### Crear la imagen

```
docker build -t ms-eureka:latest .
```

### Crear la network
En el caso que ya se haya creado la network omitir este paso

```
docker network create challenge-nttdata
```

### Ejecutar la imagen

```
docker run -d -p 8761:8761 --name ms-eureka --net challenge-nttdata ms-eureka:latest
```