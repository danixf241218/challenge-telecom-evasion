# challenge-telecom-evasion

# Informe de Análisis de Evasión de Clientes (Churn)
## - Introducción
El objetivo de este análisis es estudiar la **evasión de clientes (Churn)** en la empresa TelecomX, identificando los factores que influyen en la decisión de un cliente de cancelar su servicio o no.  
El análisis permitirá comprender patrones de comportamiento y ofrecer estrategias para reducir la evasión.
## - Limpieza y Tratamiento de Datos
Se realizaron los siguientes pasos:

1. Importación de datos desde un archivo .json a un DataFrame.
2. Normalizacion de los datos.
3. Identificación y tratamiento de valores faltantes (NaN):
   - Se hizo el tratamiento de datos de tiño string a float
   - Tratamiento de valores faltantes en otras columnas numéricas si existían.
4. Limpieza de texto:
   - Eliminación de espacios en blanco.
   - Conversión de texto a minúsculas.
5. Recodificación de variables:
   - `'yes'` → 1, `'no'` → 0 en columnas binarias.
   - `'no internet service'` → `'no'`.
6. Preparación de columnas categóricas para análisis y visualización.
