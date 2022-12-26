# Datos de prueba para el 'Validador web LADM-COL'
Conjunto de datos de prueba para subir al 'Validador web LADM-COL'.

Estos datos de prueba han sido construidos con el fin de ilustrar de manera sencilla ciertos escenarios que pueden presentarse durante una sesión de validación de reglas de calidad.

Recuerda que la aplicación permite validar datos en formato **XTF** (archivo de transferencia de [INTERLIS](https://www.interlis.ch/en)), [**GeoPackage**](https://www.ogc.org/standards/geopackage) (archivo de base de datos avalado por el OGC) y **ZIP** (archivo comprimido con un único XTF o GeoPackage al interior).



| Archivo                                                      | Modelo        | CaracterísticaS                                              | Reglas sugeridas |
| ------------------------------------------------------------ | ------------- | ------------------------------------------------------------ | ---------------- |
| [lc12_wrong_extent.gpkg](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/raw/main/data/lc12_wrong_extent.gpkg) (1.9MB) | Lev. Cat. 1.2 | El terreno no está dentro del cubrimiento de la proyección Origen Nacional. | IGAC-R0001       |
| [lc12_valid.xtf](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/blob/main/data/lc12_valid.xtf) (16.4kB) | Lev. Cat. 1.2 | Archivo válido. No genera error en ninguna regla.            | Todas            |
| [lc12_invalid.xtf](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/blob/main/data/lc12_invalid.xtf) (10.7kB) | Lev. Cat. 1.2 | Archivo inválido. Genera errores en algunas reglas.          | Todas            |
| [lc12_chia_56MB.gpkg.zip](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/raw/main/data/lc12_chia_56MB.gpkg.zip) (14.9MB-->56.3MB) | Lev. Cat. 1.2 | Archivo con casi 30.000 terrenos y más de 40.000 linderos. Inválido. Genera errores en algunas reglas. Fuente: IGAC. | Todas            |
| [ric01_wrong_extent.xtf](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/raw/main/data/ric01_wrong_extent%20.gpkg) (969.7kB) | RIC 0.1       | El terreno no está dentro del cubrimiento de la proyección Origen Nacional. | IGAC-R0101       |
| ric01_valid.xtf                                              | RIC 0.1       | Archivo válido. No genera error en ninguna regla.            | Todas            |
| ric01_invalid.xtf                                            | RIC 0.1       | Archivo inválido. Genera errores en algunas reglas.          | Todas            |

*Nota: Para descargar los XTFs, te aconsejamos dar clic derecho y elegir "Guardar como...".*

#### Archivos que no pueden cargarse al Validador web LADM-COL

Algunos archivos XTF, GPKG y ZIP no pueden cargarse a la aplicación porque pueden tener **problemas de formato**. Al intentar cargarlos, el Validador web LADM-COL los identificará e impedirá iniciar una validación de reglas de calidad sobre ellos.

Por ejemplo, un ZIP que no contiene archivos en su interior o una GeoPackage genérica que no tiene la estructura de ningún modelo LADM-COL, serán rechazados en una primera instancia, que llamamos de **pre-validación**.

A continuación disponemos para ti un conjunto de archivos que no superarán la etapa de pre-validación:

 + [Archivos XTF con problemas de formato](https://github.com/Geoideal/pre_validador_de_archivos/tree/main/data/xtf).
 + [Archivos GeoPackage con problemas de formato](https://github.com/Geoideal/pre_validador_de_archivos/tree/main/data/gpkg).
 + [Archivos ZIP con problemas de formato](https://github.com/Geoideal/pre_validador_de_archivos/tree/main/data/zip).
