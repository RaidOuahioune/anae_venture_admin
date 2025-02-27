# Docker Django React Postgres Minimal template


## Technologies

1. [Docker](https://docs.docker.com/engine/install/) & docker compose
2. [Django 4](https://www.djangoprojects.com/) & [Django rest framework](https://www.django-rest-framework.org/)
3. [React](https://react.dev/) (option mode)
4. [Vite](https://vitejs.dev/)
5. [Postgres 16](https://www.postgresql.org/)

All docker images using an [alpine](https://alpinelinux.org/about/) version

## Run projects

1. create a .env file on projects root and add SECRET_KEY variable (for django settings)
2. Launch docker
3. Open terminal and run command

```shell
docker compose up
```

3. Go to application

- Frontend at [localhost:3000](http://localhost:3000)
- Backend at [localhost:8000](http://localhost:8000)
- Django [administration](http://localhost:8000/admin)

## Run django command

For using a manage.py command, need to run it inside docker

```shell
docker compose run backend sh -c "python manage.py foo"
```
