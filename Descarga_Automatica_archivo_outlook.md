# Flujo de caja de descarga de los archivos de outlook
### *When a new email arrives (V3)*

![image](https://github.com/Miguelapp10/Automatizacion_descarga_archivo_notificar_Power_automate/assets/114699192/41e6189a-6295-4c59-9da5-dcf6e88be820)

Estos son los dos factores mas importantes:
- Folder: Seleccionar el forder  que llega el correo de las otras areas
- Subject Filter : Poner el asunto de manera, pero que sea corto y inicial.
- Include Attachments: Yes
- Only with Attachments: Yes
  
*Recomedacion*
Crear un Carpeta y una regla en outlook para mover todos los correos estandarizados hacia esa carpeta para evitar inconveniente.

### *Apply to each / Create file*
![image](https://github.com/Miguelapp10/Automatizacion_descarga_archivo_notificar_Power_automate/assets/114699192/64ac0cf7-532c-48fb-9454-37d6104cdd62)

- Apply to each: @{triggerOutputs()?['body/attachments']}
- Site Address: el nombre de sharepoint de tu grupo
- Folder Path : la ubicacion que desearia en donde este los archivos
- File Name: @{items('Apply_to_each')?['name']}
- File Content: @{items('Apply_to_each')?['contentBytes']}
