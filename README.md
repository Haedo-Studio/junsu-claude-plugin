# Junsu para Claude

Marketplace del plugin de [Junsu](https://junsu.es) para Claude. Con él, Claude lee
los pasos, los requisitos y las evidencias de un Proyecto de Junsu y prepara cambios
que ves en una vista previa antes de guardarlos. Junsu conserva los permisos, la
metodología, el cálculo y la revisión por una persona de las filas que guarda el
agente; las observaciones y sus respuestas se guardan al momento. Sirve en Claude.ai,
Claude Desktop, Cowork y Claude Code.

- Guía pública, con ejemplos y solución de problemas:
  [junsu.es/guias/claude](https://junsu.es/guias/claude).
- Qué datos trata Junsu y cómo: [junsu.es/privacidad](https://junsu.es/privacidad).

El repositorio es público y no lleva secretos. Para conectar el conector necesitas una
cuenta de Junsu: cada conexión trabaja sobre un único Proyecto, con tus permisos.

## Instalación en Claude

1. En Claude, abre **Customize → Plugins** y elige **Add → Add marketplace**.
2. Escribe `Haedo-Studio/junsu-claude-plugin` y confírmalo.
3. Activa **Sync automatically** en el marketplace para recibir cada versión nueva.
4. Añade el plugin **Junsu**. En su pestaña **Connectors**, añade el conector `junsu`
   y conéctalo: Junsu te pedirá iniciar sesión y elegir el Proyecto y el acceso.

Claude Code recibe el plugin sincronizado con tu cuenta la próxima vez que inicias
sesión con ella.

## Solo en Claude Code

```
/plugin marketplace add Haedo-Studio/junsu-claude-plugin
/plugin install junsu@junsu
```

Después, `/mcp` conecta el servidor `junsu` e inicia sesión en Junsu. Claude Code no
actualiza este marketplace por defecto: activa **Enable auto-update** en `/plugin` →
**Marketplaces** → `junsu`, o actualiza a mano con `/plugin marketplace update junsu`.

Este repositorio se genera desde Junsu en cada versión del plugin. No se edita a
mano: los cambios se hacen en Junsu.

Sus ficheros se publican con licencia MIT (`LICENSE`). La licencia cubre solo el
plugin y este repositorio, no Junsu ni su servidor.
