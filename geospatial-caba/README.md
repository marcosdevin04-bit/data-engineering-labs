# Geoespacial con GeoPandas — CABA

Abrir `UT4_12_Geoespacial_Completo.ipynb` y ejecutar las celdas en orden desde esta carpeta. Las fuentes de entrada, el extracto de red y los resultados están incluidos; `requirements.txt` registra el entorno usado.

Incluye análisis de CRS, áreas, mapas, SUACI por habitante, joins espaciales, cobertura SUBTE, `sjoin_nearest`, Folium y los cinco extras: grilla hexagonal estimada, rutas peatonales de red acotadas al sur de la ciudad, escenarios de overlay, mapa interactivo y comparación de formatos/rendimiento. Las respuestas y advertencias de interpretación están en el notebook.

Los registros SUACI corresponden a 2013–2015. Los contactos por hexágono se estiman distribuyendo totales de barrio según población/área; no son puntos observados. El extracto de red peatonal OSM se limita a tres barrios y estaciones cercanas. Estos resultados sirven para practicar el flujo geoespacial, no como diagnóstico actualizado ni como propuesta de infraestructura.

El mapa base de contexto atribuye datos a OpenStreetMap y CARTO. Los extractos OSM requieren conservar la atribución y cumplir ODbL. Las condiciones de reutilización de los datos municipales deben confirmarse en sus fuentes; se incluyen los enlaces y hashes en `data/fuentes.json` y `data/fuentes_extras.json`.

Para ejecutar: `python -m pip install -r requirements.txt` y abrir el notebook con Jupyter. Los mapas HTML usan Leaflet y mosaicos externos y requieren conexión al abrirse; el análisis y las capas están guardados localmente.

Consigna: https://juanfkurucz.com/ucu-id/ut4/12-geoespacial/