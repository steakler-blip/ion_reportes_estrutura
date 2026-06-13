La carpeta principal tiene el nombre del reporte a trabajar, podrían existir 2 archivos de excel con la estructura de datos y la configuración de los campos, y 1 carpeta llamada CATALOGOS.

El nombre del reporte corresponde al nombre de la primera pestaña del archivo layout.

Si hay 2 archivos excel en la carpeta, es porque uno de los archivos excel puede contener comentarios del usuario acerca del mapeo de los campos y otras consideraciones, el otro, es la última versión del layout y esta identificado con el subfijo "ultimaVersion". Se deben de comparar en busca de inconsistencia en el número de campos y la configuración y nombre de estos, si no existen 2 archivos excel, entonces solo se considera el archivo "ultimaVersion".

El layout del reporte puede hacer referencia a algunos de los catalogos que se encuentran en la carpeta de CATALOGOS.

Identificar la fuente de datos, si es una tabla o vista, generar el script para insertar 100 datos "dummy", si la fuente es un lambda, generar el excel con los 100 datos "dummy". La finalidad es poder ejecutar el SP y validar el resultado final.