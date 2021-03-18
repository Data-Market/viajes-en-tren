# Datasets de Viajes en Tren

<a href="https://datamarket.es">
  <img src="https://datamarket.es/media/banners/viajes-en-tren-banner.png">
</a>

## Descripción

Billetes de tren con todo su árbol de precios y plazas disponibles para las __principales rutas de Alta Velocidad (AVE) en España__. 

Las características de este dataset son las siguientes:

* __Frecuencia de actualización__: actualizado cada 4h
* __Volumen estimado__: 15.000 registros diarios
* __Histórico__: desde 2018

El dataset completo se puede adquirir en [DataMarket](https://datamarket.es/#viajes-en-tren-dataset), plataforma de referencia de datos externos en España. 

Este repositorio contiene los siguientes recursos:

* La documentación completa del dataset.
* Una muestra representativa del mismo disponible para su evaluación y uso gratuito.

## Muestra

La muestra se encuentra disponible para descarga en el siguiente [link](https://github.com/Data-Market/viajes-en-tren/blob/main/viajes-en-tren-sample.csv).

## Documentación

A continuación se muestran las columnas de las que consta el dataset junto con su descripción.

| nombre | tipo | descripción | ejemplo |
|--------|------|-------------|---------|
| arrival | datetime | Fecha y hora de llegada del tren a la estación de destino. | 2020-12-08 17:06:48 |
| company | str | Empresa que ofrece el servicio de transporte ferroviario (encriptado). Estará disponible tras la suscripción al dataset. | 2991AADB8BA01C768CFFE9329B46049A |
| departure | datetime | Fecha de salida del viaje en tren. | 2020-12-08 15:05:00 |
| destination | str | Estación de destino del trayecto. | BARCELONA |
| duration | float | Duración del trayecto (en horas). | 2.03 |
| fare | str | Tipo de tarifa de la opción más económica. | Flexible |
| insert_date | datetime | Fecha de extracción del viaje. | 2020-12-08 12:00:00 |
| meta | json | Árbol completo de precios y plazas para todas las clases y tarifas. | {"Turista": {"Flexible": {"price": 55.9, "seats": 76}}, "Turista Plus": ...}} |
| origin | str | Estación de origen del trayecto. | MADRID |
| price | float | Menor precio disponible para el trayecto, en €. | 55.9 |
| seats | int | Número de plazas disponibles para la opción más económica disponible. | 76 |
| vehicle_class | str | Clase del billete de menor precio disponible en el momento de la extracción. | Turista |
| vehicle_type | str | Tipo de tren. | AVE |
