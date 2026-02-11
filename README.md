# sdr-bizkaia
Código en Google Earth Engine para preparar datos espaciales en Bizkaia: selección de límites provinciales, microcuencas HydroBASINS nivel 12, CORINE Land Cover 1990 y 2018 y MDE SRTM, recorte al área de estudio y exportación a Google Drive para análisis de erosión y sedimentos.

# Datos para modelización SDR en Bizkaia

Repositorio con código de Google Earth Engine (GEE) para preparar las capas espaciales utilizadas en un estudio de tasa de entrega de sedimentos (SDR) en Bizkaia.

El script principal:

- Selecciona la provincia de Bizkaia a partir de los límites administrativos GAUL (nivel 2).
- Obtiene las microcuencas de alta resolución (HydroATLAS/HydroBASINS, nivel 12) que intersectan Bizkaia.
- Recorta la cobertura y uso del suelo CORINE Land Cover (1990 y 2018) al ámbito de las microcuencas.
- Recorta el modelo digital de elevación SRTM al área de estudio.
- Visualiza las capas en el visor de GEE.
- Exporta microcuencas (SHP) y capas raster (CORINE y MDE en EPSG:25830) a Google Drive para su uso posterior en modelos de erosión y sedimentación.

## Uso

1. Abrir el script en el Code Editor de Google Earth Engine.
2. Ajustar, si es necesario, la carpeta de salida `GEE_Exports` en Google Drive.
3. Ejecutar el script para generar las exportaciones de:
   - Microcuencas nivel 12 que intersectan Bizkaia.
   - CORINE Land Cover 1990 y 2018 recortado a Bizkaia.
   - MDE SRTM recortado a Bizkaia.

## Requisitos

- Cuenta activa en Google Earth Engine.
- Espacio disponible en Google Drive para las exportaciones.

## Cómo citar

Si utiliza este código en un trabajo científico, cite el repositorio como:

> Larrinaga López, J. (2026). Código para la preparación de datos SDR en Bizkaia (versión 1.0). Repositorio GitHub. Disponible en: https://github.com/jonlarri2127/sdr-bizkaia 
