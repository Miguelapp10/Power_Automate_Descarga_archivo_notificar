### When a file is created (properties only)

![image](https://github.com/Miguelapp10/Automatizacion_descarga_archivo_notificar_Power_automate/assets/114699192/02472687-add7-47e5-9f31-9f72f3a08ea2)

Colocar la misma ruta que has colocado anteriormente en CREATE FILE

### Post message in a chat or channel

![image](https://github.com/Miguelapp10/Automatizacion_descarga_archivo_notificar_Power_automate/assets/114699192/e9ed2d32-0877-47c9-911e-bf425bc95ab1)

- Group chat: Poner el nombre del grupo que deseas notificar
- Nuevo archivo Publicado:@{triggerOutputs()?['body/{Name}']}
- enlace : @{triggerOutputs()?['body/{Link}']}
