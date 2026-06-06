** Estructura de carpeta

El nombre del reporte es FILE_GARANTIAS_IV

El archivo excel contiene los encabezados y tipo de datos que se esperan por campo. Buscar en la columna catalogos si es que hacen referencia a alguno.

Los catalogos estan en la carpeta con ese nombre.

En la BD estan asociado a objetos con nomenclatura 142_ENT_GARANTIAS_IV.

En los entregables se debe de incluir un archivo excel con 100 registros, la información de encabezados, tipo, longitud y formato de datos estan especificados en el excel FILE_GARANTIAS_IV.

También se debe de generar una plantilla en excel con los encabezados tomados del layout. El formato de las celdas de cada columna, debe de ser coherente con lo que indica dicho layout. Cada encabezado debe de tener un comentario sencillo, que inlcuya la descripcion, la cual es tomada del mismo archivo (no importa que se tenga que hacer click en la celda de cada encabezado.). Si la columna esta asociada a 1 catalogo, se debe de considerar para esa columna que exista una lista desplegable con las claves indicadas en cada catalogo, de ser necesario incluye una hoja extra donde exista la referencia a los catalogos.

En caso de no existir ningun objeto relacionado en la base de datos:

Se requiere generación de flujo completo: estructuras bronze, silver e ion, extractor (consulta en SP silver). 

Todas las tablas creadas llevan los campos ID [uniqueidentifier not null pk default newid()] y FECHA_EXTRACCION [smalldatetime not null default getdate()]. Estos campos no se reflejan en la vista en ION

En caso de ya existir, se requiere validar que la salida de los SP, cumpla con el formato especificado en el layout. Y de no ser así, emitir los scripts para corregir lo necesario.