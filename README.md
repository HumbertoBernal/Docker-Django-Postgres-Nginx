### Instalación:

1. Crear y llenar .env

### Como correr:
 
* Para desarrollo local con docker:

```bash
docker-compose build
docker-compose exec web python manage.py migrate
docker-compose up -d
```

> Para correr comandos dentro de un contenedor usa
  `docker-compose -f local.yml run --rm django python manage.py <command>`

### Save local backup
``` 
docker cp <volume_name>:/var/lib/postgresql/data ~/Desktop/backup|-

docker cp ~/Desktop/backup|- <volume_name>:/var/lib/postgresql/data
``` 