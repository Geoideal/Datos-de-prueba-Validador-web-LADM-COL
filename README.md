# Datos de prueba para el 'Validador web LADM-COL'
Conjunto de datos de prueba para subir al 'Validador web LADM-COL'.

Estos datos de prueba han sido construidos con el fin de ilustrar de manera sencilla ciertos escenarios que pueden presentarse durante una sesión de validación de reglas de calidad.

Recuerda que la herramienta permite validar datos en formato **XTF** (archivo de transferencia de [INTERLIS](https://www.interlis.ch/en)), [**GeoPackage**](https://www.ogc.org/standards/geopackage) (archivo de base de datos avalado por el OGC) y **ZIP** (archivo comprimido con un único XTF o GeoPackage al interior).



| Archivo                               | Modelo        | Característica                                               | Reglas sugeridas |
| ------------------------------------- | ------------- | ------------------------------------------------------------ | ---------------- |
| [lc12_wrong_extent.gpkg](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/raw/main/data/lc12_wrong_extent.gpkg) (1.9MB)         | Lev. Cat. 1.2 | El terreno no está dentro del cubrimiento de la proyección Origen Nacional. | IGAC-R0001       |
| [lc12_valid.xtf](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/blob/main/data/lc12_valid.xtf) (16.4kB)                       | Lev. Cat. 1.2 | Archivo válido. No genera error en ninguna regla.            | Todas            |
| [lc12_invalid.xtf](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/blob/main/data/lc12_invalid.xtf) (10.7kB)                     | Lev. Cat. 1.2 | Archivo inválido. Genera errores en algunas reglas.          | Todas            |
| [lc12_heavy.gpkg.zip](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/raw/main/data/lc12_heavy.gpkg.zip) (14.9MB-->56.3MB) | Lev. Cat. 1.2 | Archivo pesado (casi 30.000 terrenos) e inválido. Genera errores en algunas reglas. | Todas            |
| [ric01_wrong_extent.xtf](https://github.com/Geoideal/Datos-de-prueba-Validador-web-LADM-COL/raw/main/data/ric01_wrong_extent%20.gpkg) (969.7kB)               | RIC 0.1       | El terreno no está dentro del cubrimiento de la proyección Origen Nacional. | IGAC-R0101       |
| ric01_valid.xtf                       | RIC 0.1       | Archivo válido. No genera error en ninguna regla.            | Todas            |
| ric01_invalid.xtf                     | RIC 0.1       | Archivo inválido. Genera errores en algunas reglas.          | Todas            |

