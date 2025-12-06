# Copy file to

Actions para copiar archivos.

## ¿Copy file to?

Este Actions facilita el copiado de archivos de un directorio a otro.

## Prerrequisitos

Se debe indicar con la etiqueta 'with' algunos parametros.

1. Archivo a copiar
2. Directorio destino

## Instrucciones

1. Copiar el llamado del action en el maketplace de GitHub. Recomendamos usar siempre la ultima versión.

Ejemplo:

<p align="center">
  <img width="630" height="61" alt="action" src="public/img/action.PNG">
</p>

2. Pega en tu workflow y añade la etiqueta with: añadiendo los parametros: "work_dir" y "artifact_name".

Ejemplo:

<p align="center">
  <img width="630" height="149" alt="action_with" src="public/img/action_with.PNG">
</p>

Se debe indicar el valores que corresponden. 

## Ejecución por consola

1. cd ${{ inputs.work_dir }}
2. cp -R ${{ inputs.file }} ${{ inputs.to }}
3. cd ${{ inputs.to }} && ls -l