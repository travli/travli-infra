# Travli Infrastructura

Repositorio encargado de gestionar la infraestructura necesaria para el desarrollo y despliegue de Travli.

Actualmente contiene la configuración de los servicios de infraestructura utilizados durante el desarrollo local.

## Infraestructura local

La infraestructura local se ejecuta mediante Docker Compose.

| Servicio | Puerto | Uso |
|---|---:|---|
| Redis Weather | `6379` | Cache de la Weather API |
| Redis Location | `6380` | Cache de la Location API |


## Uso

### Levantar la infraestructura

Desde el directorio `docker/`:

```bash
docker compose up -d
```

### Comprobar los servicios

```bash
docker compose ps
```

### Detener los servicios

```bash
docker compose down
```

Los datos de Redis se almacenan en volúmenes Docker para mantener la información entre reinicios de los contenedores.

