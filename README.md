# ETL Bebidas — Landing

Página principal con acceso a los catálogos de pedidos mayorista y minorista.

## Editar

Todo está en `site/index.html`. Al final del archivo, en el bloque `EDITÁ ACÁ`:

- `LINKS.mayorista` / `LINKS.minorista`: links a los catálogos de pedidos.
- `MARCAS`: marcas que aparecen en la franja.

## Deploy en Railway

1. New Project → Deploy from GitHub repo → elegir este repo.
2. Railway detecta el `Dockerfile` y sirve la página con Caddy en el puerto `$PORT`.
3. Settings → Networking → Generate Domain (o agregar el dominio propio).

## Probar local

```sh
docker build -t etl-landing . && docker run -p 8080:8080 etl-landing
```
