# TP4 - Redes convolucionales para clasificar lesiones de piel (ISIC)

Clasificación de imágenes dermatoscópicas de 9 clases con una CNN en PyTorch, comparada con una MLP. Incluye análisis exploratorio, eliminación de duplicados, split estratificado, experimentos de arquitectura, data augmentation hecha a mano y evaluación final en test.

## Contenido

- `CNN_en_Skin_Dataset_PerezRaffo(1).ipynb`: notebook ejecutado, con outputs y análisis.
- `requirements.txt`: dependencias.

El dataset no está incluido en este repositorio.

## Cómo reproducirlo

### En Google Colab

1. Abrir el notebook en Colab.
2. Ejecutar todas las celdas (Entorno de ejecución → Ejecutar todas).

La primera celda descarga automáticamente la carpeta `data/Split_smol` desde el repositorio del TP (`cselmo/CNN-en-Skin-Dataset`) y se posiciona en ella, así que no hace falta subir nada.

### En una computadora local

```bash
git clone <url-de-este-repo>
cd <carpeta-del-repo>
pip install -r requirements.txt
jupyter notebook CNN_en_Skin_Dataset_PerezRaffo.ipynb
```

Al ejecutar la primera celda, el notebook descarga el dataset con `git` (tiene que estar instalado).

## Notas

- Se usaron las constantes por defecto de la sección 0 (semillas, épocas, tamaños de imagen, semilla del split = 42). No se modificó ninguna.
- El cómputo tarda unos 20-25 minutos en CPU.
- Los resultados pueden variar levemente entre ejecuciones y entre máquinas.
