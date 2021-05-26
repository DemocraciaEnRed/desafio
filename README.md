##  Programación en DeR
En DeR te animamos a que cuestiones, ofrezcas aportes, o tengas impulso propio a cambiar esquemas en función a la mejora continua en diversas áreas: UX, seguridad, metodologías, lógicas en back y front, eficiencia/performance, etc.

Tener miradas críticas o discusiones para mejorar, hacer bug-hunting, aportes a la seguridad o integridad del codigo son realmente apreciados en nuestro equipo. 

## Desafío
El objetivo de este desafío es evaluar la capacidad del solicitante para llevar al cabo requerimientos de desarrollo sobre plataformas existentes hechas en [Node.js](https://nodejs.org/) y [React](reactjs.org/).

Aspectos a tener en cuenta a la hora de crear código:
- Dejar comentarios en el código sobre lo que hacen las rutinas para que sea más fácil de leer
- Utilizar los mismos patrones de desarrollo que la plataforma que se está modificando (apreciamos aportes y mejoras a los mismos)
- Seguir estándares de cada tecnología

Este desafío utilizaremos como "base" el repositorio de la [página web](https://democraciaenred.org/) de DeR. El repositorio se encuentra aqui: [https://github.com/DemocraciaEnRed/website](https://github.com/DemocraciaEnRed/website)

Puede clonarlo localmente con Git para comenzar.

```
$ git clone https://github.com/DemocraciaEnRed/website
```

Pueden usar el siguiente `.env` en el root del proyecto

```
HOST=https://democraciaenred.org
JWT_SECRET=LnmaI6Ezcw4oeSmO8Zl0GUe1POmJSRUIw9Yxl09p
MAILGUN_API_KEY=thisIsASecret
MAILGUN_DOMAIN=thisIsASecret
MAILGUN_PUBLIC_KEY=thisIsASecret
MEDIUM_URL=https://medium.com/multitudes
PORT=3000
YOUTUBE_API_KEY=thisIsASecret
GOOGLE_UA=thisIsASecret
```

### Formato de presentación

1. Crear un fork de [https://github.com/DemocraciaEnRed/website](https://github.com/DemocraciaEnRed/website)
2. Llevar a cabo los cambios. 
3. Enviar el link al repositorio para que lo podamos ver!

### Requerimientos

Simulando que queremos hacer cambios en nuestra web, emulamos los siguiente requerimientos

__Backend:__
Crear una ruta GET en la URL `/api/traer-usuarios` que devuelva un JSON con los primeros 4 ítems con `userId` 6 de https://jsonplaceholder.typicode.com/posts. 

__Frontend:__
Crear una nueva sección en la home después de la sección "¿Qué hacemos?", con título Usuarios, que muestre los ítems devueltos por `/api/traer-usuarios` en recuadros con sus respectivos título y texto (`title` y `body` del JSON). Utilizar flexbox para que sea mobile friendly.

__BONUS__
Este punto es opcional pero nos alegraría mucho saber cómo lo resolverías, con código o no. Lo importante es ver qué cosas tendrías en cuenta en cada caso.

- Supongamos que agregamos en la nueva sección un campo de búsqueda de palabras en los títulos de los posts y los devuelva. (*++Bonus* si lográs hacer que también se puedan ver datos del usuario/a autor/a del post, podés usar [https://jsonplaceholder.typicode.com/users](https://jsonplaceholder.typicode.com/users) y/o [https://jsonplaceholder.typicode.com/users/{userId}](https://jsonplaceholder.typicode.com/users/{userId}))
