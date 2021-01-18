# Viajes en Tren

Billetes de tren con todo su árbol de precios y plazas disponibles para las principales rutas de Alta Velocidad (AVE) en España. Este dataset se puede adquirir en [Data Market](https://datamarket.es/#viajes-en-tren-dataset), plataforma de referencia de datos externos en España. Puede consultar nuestro catálogo de datos en la siguiente url: [datamarket.es](https://datamarket.es/)

A continuación se muestran las columnas de las que consta el dataset en el formato __nombre_columna__: __ejemplo_columna__, donde ejemplo_columna representa posibles valores que se pueden encontrar en dicha columna.

| nombre        | tipo     | descripción                                                                                                              | ejemplo                                                                       |
|---------------|----------|--------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| company       | str      | Empresa que ofrece el servicio de transporte ferroviario (encriptado). Estará disponible tras la suscripción al dataset. | 2991AADB8BA01C768CFFE9329B46049A                                              |
| origin        | str      | Estación de origen del trayecto.                                                                                         | MADRID                                                                        |
| destination   | str      | Estación de destino del trayecto.                                                                                        | BARCELONA                                                                     |
| departure     | datetime | Fecha de salida del viaje en tren.                                                                                       | 2020-12-08 15:05:00                                                           |
| arrival       | datetime | Fecha y hora de llegada del tren a la estación de destino.                                                               | 2020-12-08 17:06:48                                                           |
| duration      | float    | Duración del trayecto (en horas).                                                                                        | 2.03                                                                          |
| vehicle_type  | str      | Tipo de tren.                                                                                                            | AVE                                                                           |
| vehicle_class | str      | Clase del billete de menor precio disponible en el momento de la extracción.                                             | Turista                                                                       |
| price         | float    | Menor precio disponible para el trayecto, en €.                                                                          | 55.9                                                                          |
| fare          | str      | Tipo de tarifa de la opción más económica.                                                                               | Flexible                                                                      |
| seats         | int      | Número de plazas disponibles para la opción más económica disponible.                                                    | 76                                                                            |
| meta          | json     | Árbol completo de precios y plazas para todas las clases y tarifas.                                                      | {"Turista": {"Flexible": {"price": 55.9, "seats": 76}}, "Turista Plus": ...}} |
| insert_date   | datetime | Fecha de extracción del viaje.                                                                                           | 2020-12-08 12:00:00                                                           |
