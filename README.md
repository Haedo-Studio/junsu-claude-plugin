# Junsu para Claude

Marketplace del plugin de [Junsu](https://junsu.es) para Claude: el conector de
Junsu y la guía para trabajar en un Proyecto desde Claude.ai, Claude Desktop y
Claude Code.

## Instalación

El repositorio es privado: necesitas una cuenta de GitHub con acceso de lectura.
Pídelo a Junsu.

1. En Claude, abre **Customize → Plugins** y elige **Add marketplace**.
2. Escribe `Haedo-Studio/junsu-claude-plugin`. Si Claude te lo pide, conecta tu
   cuenta de GitHub y da acceso a este repositorio a la app de Claude en GitHub.
3. Activa **Sync automatically** en el marketplace para recibir cada versión nueva.
4. Instala el plugin **Junsu** y conecta su conector desde la pestaña
   **Connectors**. Junsu te pedirá iniciar sesión y elegir el Proyecto.

En Claude Code:

```
/plugin marketplace add Haedo-Studio/junsu-claude-plugin
/plugin install junsu@junsu
```

Claude Code no actualiza este marketplace por defecto: activa **Enable auto-update**
en `/plugin` → **Marketplaces** → `junsu`, o actualiza a mano con
`/plugin marketplace update junsu`. Claude Code clona el repositorio con tus
credenciales de git: si no tienes clave SSH de GitHub, ejecuta antes
`gh auth login` y `gh auth setup-git`. Si instalaste el plugin desde Claude.ai, Claude
Code lo recibe sincronizado con tu cuenta y no necesitas estos pasos.

Este repositorio se genera desde Junsu en cada versión del plugin. No se edita a
mano: los cambios se hacen en Junsu.
