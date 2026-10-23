# UT4 — Actividad 14: Audio como dato

Abrir **UT4_14_Audio_Completo.ipynb** en Jupyter o VS Code. Ejecutar las celdas en orden desde esta carpeta. El notebook contiene explicaciones, análisis, figuras y resultados guardados.

Secciones: A (inspección), B (estandarización), C (espectrogramas y ruido), D (MFCC y CSV), E.1–E.3 (descriptores, clasificación y aumentos), F.1–F.3 (sensibilidad al SNR, comparación de pipelines y QA con semáforo), y reflexiones finales.

## Archivos incluidos

- `data/raw/fold1` a `fold10`: 200 WAV reales de UrbanSound8K.
- `data/metadata/UrbanSound8K.csv`: metadata completa de 8732 clips.
- `data/metadata/seleccion_200.csv`: selección reproducible, dos clips por clase/fold. Slot 0 define el núcleo de 100.
- `data/metadata/manifest.json`: nombres, tamaños y SHA-256 de los WAV incluidos.
- `outputs/features`: descriptores originales, etiquetados y aumentados.
- `outputs/metrics`: SNR, pipelines, evaluación, QA y umbrales; `qa_dashboard.html` se abre en el navegador.
- `outputs/figures`: figuras exportadas, también incrustadas en el notebook.
- `outputs/audio`: ejemplo estandarizado.
- `requirements.txt`: versiones de las dependencias usadas.

## Reproducir

1. Descomprimir la entrega completa conservando su estructura.
2. Instalar dependencias si faltan: `python -m pip install -r requirements.txt`.
3. Abrir el notebook con ese entorno y ejecutar todas las celdas desde la carpeta del proyecto.

Los datos incluidos permiten repetir los cálculos sin autenticarse en Kaggle. Si se eliminan archivos, la celda de carga intenta descargarlos mediante kagglehub. Una descarga nueva puede requerir credenciales privadas según la configuración de Kaggle. No se incluyen tokens ni archivos de credenciales.

El ejemplo de clasificación usa 80 clips de entrenamiento (folds 1–8) y 20 de prueba (folds 9–10). Sus 160 aumentos se generan únicamente a partir de entrenamiento. Este subconjunto no equivale al benchmark oficial sobre todos los 8732 clips. El proxy de contraste de energía en QA tampoco equivale al SNR real de las grabaciones originales.

Consigna: https://juanfkurucz.com/ucu-id/ut4/14-audio/

Datos: https://www.kaggle.com/datasets/chrisfilo/urbansound8k

Fuente original y condiciones de uso: https://urbansounddataset.weebly.com/urbansound8k.html
