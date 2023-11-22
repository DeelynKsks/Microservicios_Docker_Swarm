## Inicializar Docker Swarm

Para inicializar Docker Swarm, utiliza el siguiente comando:

```bash
docker swarm init
```
Desplegar un Stack de Servicios
Para desplegar un stack de servicios, utiliza el siguiente comando:

```bash
docker stack deploy -c docker-compose.yml mystack
```
Listar Servicios
Para listar todos los servicios en ejecución en el swarm, utiliza el siguiente comando:

```bash
docker service ls
```

Para ver los detalles de una instancia de servicio, utiliza el siguiente comando:

```bash
docker service ps mystack_web
```

Para actualizar el número de réplicas de un servicio, utiliza el siguiente comando:

```bash
docker service update --replicas=5 mystack_web
```

Para escalar un servicio, utiliza el siguiente comando:

```bash
docker service scale mystack_web=5
```