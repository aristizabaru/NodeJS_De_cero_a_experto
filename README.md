# NodeJS: De cero a experto (NOC APP)

## Acerca de

Este es un repositorio personal para ejecución de los proyectos del cursos **NodeJS: De cero a experto** de **Fernando Herrera** en Udemy. Para acceder al curso completo puede hacer [clic aquí](https://www.udemy.com/course/node-de-cero-a-experto/)

El proyecto desarrollado a continuación es un sistema de monitoreo (NOC). En el proceso se exploran fundamentos de Arquitectura Limpias entre otros conceptos más de arquitectura de software.

## Requerimientos

- Node 20.9.0 LTS
- Docker

## Instalación del proyecto

Para instalar el proyecto siga los siguientes pasos

Instalar módulos o dependencias

```
npm install
```

## Ejecución del proyecto

Para ejecutar el proyecto se deben seguir los siguientes pasos:

1. Clonar el archivo `.env.template` a `.env`
2. Configurar variables de entorno

```
PORT=3000

MAILER_EMAIL=
MAILER_SECRET_KEY=

PROD=false

```

3. Levantar las bases de datos

```
docker compose up -d

```

4. Generar las migraciones de Prisma a la base de dato de Postgres

```
npx prisma migrate dev

```

5. Correr el proyecto usando alguno de los siguientes scripts según el entorno

Ejecutar entorno de desarrollo

```
npm run dev
```

Ejecutar entorno de producción

```
npm start
```

## Testing

Para ejecutar correctamente los test debe hacer una copia del .env.template a .env.test y configurar las variables de entorno de pruebas
