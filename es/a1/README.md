# Parte II
### El desafío del acortador de URL's

Tu misión será crear una REST API que sirva para crear links cortos, estos son más fáciles de compartir vía sms o por mensajes, a la par que permiten crear analytics sobre el consumo de dicho servicio.

Crea un repositorio para tu proyecto, puedes usar Github, Gitlab, Bitbucket, etc.

Cuando termines por favor compartenos tu repositorio y de ser posible los links de tu aplicación si lograste desplegarla.

+puntos extra si usas docker.

Si has visto acortadores de ligas como [bit.ly](https://bit.ly), [cutt.ly/](https://cutt.ly/) seguramente estarás familiarizado con el problema, si tienes una liga con parámetros en la url enorme y la quieres compartir por un chat o sms, los acortadores de url's son tu herramienta indicada, te recomendamos investigar los productos antes mencionados antes de comenzar con tu desarrollo.

Adicionalmente, quieres guardar información de los usuarios con quienes compartiste el link, datos como la dirección IP, navegador, cuántas veces ha abierto el link. etc.

### Requerimientos
- Como un usuario quiero crear una cuenta en la api del shortener.
  Criterios de aceptación:
    - Necesito un correo, contraseña mínimo para poder registrarme
    - Debe tener validaciones, no se puede repetir el correo.
    - Debe poder generar un token para poder interactuar con los demás endpoints de la API.
- Cómo usuario puedo autenticarme y obtener un token que puedo usar para acceder al listado de mis links.
  CdA:
    - Este token debe ser enviado como encabezado de autenticación.
    - El endpoint `/links` me permite ver sólo los links que el usuario loggeado creo.
- Cómo usuario loggeado puedo crear un nuevo link corto.
  CdA:
    - El endpoint `POST /links` Recibe como parámetro la url que deseo acortar.
    - Automáticamente se debe generar un código con el cual puedo identificar el link.
    - El código generado debe ser una cadena alfanumérica que me permita evitar colisiones.
    - El código no debe ser repetido.
    - El código debe ser generado con algún algoritmo personalizado (ver [hashids](https://hashids.org/) como referencia).
    - No usar alguna gema que automatice la generación del código.
    - La lóngitud mínima del código debe ser de 6 caracteres, ejemplo: `3kTMd2`.
    - El link corto debe estar asociado al usuario loggeado (por el token).


- Cada que comparto el link corto (ejemplo: https://myapp.com/GH53F3) y este link ha sido abierto, el servicio debe redirigir al link original,
  CdA:
    - El servicio debe guardar la data de cada visita, información como: `dirección IP`, `navegador`, `Sistema operativo (si s posible`, `fecha`.
    - Se debe contabilizar las veces que el link ha sido abierto.
- Cómo usuario puedo eliminar o editar los links que he creado.
  CdA:
    - El endpoint `PUT /links/:código` me permite editar la url del link.
    - El endpoint `DELETE /links/:código` me permite eliminar un link.

- Cómo desarrollador, mi código debe tener pruebas de modelos y requests como mínimo, usando RSpec o minitest.

- Cómo desarrollador debo publicar mi código en un repositorio en github, gitlab o bitbucket.

- Cómo desarrollador debe publicar mi aplicación en un entorno de pruebas como Heroku.