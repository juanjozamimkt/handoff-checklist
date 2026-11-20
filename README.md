# HANDOFF y CHECKLIST

Dos archivos para cambiar de chat sin explicarle todo de nuevo a tu IA. Son los que uso en todos mis proyectos.

## Para qué sirven

Una IA no se acuerda de un chat a otro. Y adentro de un mismo chat relee todo cada vez que le escribís, también lo que ya descartaste. Por eso un chat largo y con varios temas mezclados empieza a contestar peor, y uno nuevo arranca sin saber nada.

Con estos dos archivos podés cerrar el chat largo sin perder nada:

- `HANDOFF.md` (en inglés, «pasar la posta») dice dónde quedamos, qué decidimos y por qué, qué falta y cómo se retoma.
- `CHECKLIST.md` es la lista de lo hecho y lo pendiente, separada por a quién le toca.

Los escribe y los actualiza la IA. Vos los leés y le corregís lo que haya anotado mal.

## Cómo se usan

### Si tu IA puede leer y escribir archivos

Es el caso de Claude Code, de Codex y de otras parecidas.

1. Copiá `HANDOFF.md` y `CHECKLIST.md` a la carpeta de tu proyecto. También podés pegarle el link de este repo a tu IA y escribirle: «Leé este repo y armame el HANDOFF y la CHECKLIST de este proyecto.»
2. Cuando el chat ya viene largo, o cuando cambiás de tema, escribile: «Actualizá el HANDOFF y la CHECKLIST.»
3. Limpiá el contexto. En Claude Code se hace con `/clear`, que arranca una conversación nueva y vacía. En otras IA, abrí un chat nuevo.
4. Escribile: «Leé el HANDOFF y la CHECKLIST y decime dónde quedamos y qué me toca.»

### Cuándo conviene limpiar

En Claude Code, por defecto, al contexto le entra un millón de tokens (un token es un pedazo de palabra). Pero la IA empieza a contestar peor mucho antes de llenarlo: entre los 250.000 y los 500.000 tokens, según la tarea y a quién le preguntes. Un buen punto medio es actualizar los dos archivos y limpiar en algún momento de ese tramo.

Para ver cuánto llevás usado, escribí `/context`.

### Si tu IA no guarda archivos

Con un chat común de ChatGPT, Claude o Gemini se hace igual, copiando y pegando.

1. Antes de cerrar el chat, pegale la plantilla de `HANDOFF.md` y pedile que la complete con lo que hicieron.
2. Guardá ese texto en una nota o en un documento.
3. Abrí un chat nuevo y pegalo como primer mensaje.

## Que lo haga sola

Para no pedírselo cada vez, copiá el texto de `REGLAS.md` en las instrucciones fijas de tu IA. En Claude Code es el archivo `CLAUDE.md`. Otras IA tienen un archivo o un campo parecido para sus instrucciones.

Con esas reglas, la IA lee los dos archivos al abrir cada chat y los actualiza antes de cerrarlo.

## Qué anotar

- Cada decisión va con su porqué. «Quedó el fondo crema porque el oscuro le pareció de bar» te ahorra discutirlo de nuevo en tres semanas.
- Lo que se descartó también se anota, con su motivo, para que la IA no lo vuelva a proponer.
- Cada pendiente tiene dueño: vos, la IA o un tercero (un cliente, un proveedor).
- El HANDOFF termina con la prompt para la próxima sesión, que es el mensaje ya escrito con el que arranca el chat nuevo.
- La charla queda afuera. Si anotás todo lo que se dijo, armaste otro chat largo.
- Las contraseñas y las claves tampoco van.

## Cómo ordenarse

- Usá un chat por tema y una carpeta por proyecto.
- Si un proyecto tiene dos frentes que avanzan por separado, dale un HANDOFF a cada uno, por ejemplo `HANDOFF-web.md` y `HANDOFF-anuncios.md`.
- Cuando una versión quede vieja, movela a una carpeta `anteriores/` en vez de borrarla.

## Ejemplo

En la carpeta `ejemplo/` hay un HANDOFF y una CHECKLIST completos, de un proyecto inventado, para ver cómo quedan.

## Licencia

MIT. Usalos y cambialos como quieras.

Juan, tu AdsBroder.
[adsbroder.com](https://adsbroder.com) y [@adsbroder](https://www.instagram.com/adsbroder) en Instagram.
