# Clase 12 — Geoespacial con GeoPandas

Abrir `UT4_12_Geoespacial_Completo.ipynb` y ejecutar las celdas desde esta carpeta. Las entradas de referencia, red peatonal y capas auxiliares están incluidas en `data/`; los resultados se guardan en `outputs/`.

El notebook resuelve A–D, nearest, reflexiones finales y los cinco extras: hexgrid estimado, rutas por una red peatonal acotada, overlays, mapa avanzado interactivo e IO/performance. Incluye respuestas, mapas, CSV y capas GeoParquet.

El ejercicio mezcla fuentes con fechas distintas: los registros SUACI son 2013–2015, mientras que la red/zonas OSM son un extracto más reciente. Las estimaciones por hexágono redistribuyen población/contactos proporcionalmente al área; no son observaciones geocodificadas. La red peatonal se limita al sur de CABA y su entorno de estaciones. Es una práctica metodológica, no un diagnóstico actual de la ciudad ni una propuesta de obras.

Para reproducir: `python -m pip install -r requirements.txt` y ejecutar en orden con Jupyter. Los mapas Folium requieren Internet para descargar Leaflet/tiles al abrir el HTML; los cálculos, capas y figuras estáticas están incluidos.

Se mantienen las atribuciones y fuentes originales en el notebook y `data/fuentes*.json`. Verificar las condiciones de redistribución de cada dataset antes de publicarlo fuera de este uso académico.
