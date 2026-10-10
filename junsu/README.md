# Junsu

Trabaja en un Proyecto de Junsu desde Claude: recorre sus pasos, consulta sus
datos y evidencias, prepara cambios, revísalos con una vista previa y guárdalos, y
responde a las observaciones del certificador.

## Uso

Tras añadir el plugin, conecta el conector Junsu desde la pestaña Connectors del
plugin. Junsu te pedirá iniciar sesión y elegir el Proyecto y si la conexión es de
lectura o de lectura y escritura. Cada conexión trabaja sobre un único Proyecto.
Para pasar a otro, pídeselo a Claude: te dará un enlace a Junsu donde lo eliges,
sin desconectar el conector.

## Datos

El plugin envía a Junsu las consultas y cambios que Claude hace en tu nombre, con
tus permisos en el Proyecto. Junsu registra cada operación con tu usuario, y las
filas que escribe el agente quedan pendientes de revisión en Junsu. El plugin no
guarda datos por sí mismo.
