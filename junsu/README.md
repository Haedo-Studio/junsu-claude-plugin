# Junsu

Trabaja en un Proyecto de Junsu desde Claude: recorre sus pasos, consulta sus
datos y evidencias, prepara cambios, revísalos con una vista previa y guárdalos, y
responde a las observaciones del certificador.

La guía pública explica cómo conectarlo, qué pedirle y qué hacer si algo falla:
[junsu.es/guias/claude](https://junsu.es/guias/claude).

## Uso

En Claude, añádelo desde el directorio o desde **Customize → Plugins** con el
marketplace `Haedo-Studio/junsu-claude-plugin`. En Claude Code:

```
/plugin install junsu --marketplace Haedo-Studio/junsu-claude-plugin
```

Tras añadir el plugin, conecta el conector Junsu desde la pestaña Connectors del
plugin. Junsu te pedirá iniciar sesión y elegir el Proyecto y si la conexión es de
lectura o de lectura y escritura. Cada conexión trabaja sobre un único Proyecto.
Para pasar a otro, pídeselo a Claude: te dará un enlace a Junsu donde lo eliges,
sin desconectar el conector.

## Qué contiene y qué contacta

El plugin son ficheros de texto y un logo: la guía `junsu-project`, que explica a
Claude cómo recorrer un Proyecto, y la configuración del conector. No ejecuta nada en
tu equipo ni lleva secretos. Solo contacta el servidor MCP de Junsu que declara
`.mcp.json` (`https://junsu.es/mcp`) y, para que inicies sesión, el OAuth de Junsu
en `https://junsu.es`.

## Datos

El plugin no guarda datos por sí mismo. Claude envía a Junsu las consultas y los
cambios que hace en tu nombre, con tus permisos en el Proyecto, y Junsu le devuelve
lo que pide del Proyecto: datos de sus pasos, fragmentos de documentos y
observaciones. Junsu registra cada escritura con tu usuario. Las filas que guardan
las herramientas `save_*` pasan antes por una vista previa y quedan pendientes de
revisión en Junsu; las observaciones y sus respuestas se guardan al momento. Cómo
trata Junsu estos datos: [junsu.es/privacidad](https://junsu.es/privacidad).

## Licencia

Los ficheros de este plugin se publican con licencia MIT (`LICENSE`). La licencia
cubre solo el plugin, no Junsu ni su servidor.
