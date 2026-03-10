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

##  Análisis Exploratorio de Datos
Se analizaron las siguientes variables categóricas en relación con `churn`:  
`gender`, `partner`, `dependents`, `phoneservice`, `multiplelines`, `internetservice`,  
`onlinesecurity`, `onlinebackup`, `deviceprotection`, `techsupport`, `streamingtv`,  
`streamingmovies`, `contract`, `paperlessbilling`, `paymentmethod`.

##  Conclusiones e Insights
- Los contratos **month-to-month** presentan la mayor evasión; contratos largos reducen churn.
- Clientes que utilizan **electronic check** muestran mayor probabilidad de cancelar.
- Tener **pareja o dependientes** reduce la probabilidad de churn.
- Servicios como **fibra óptica**, streaming de TV o películas aumentan la evasión.
- El Género y el servicio telefónico no muestra ninguna influencia significativa para la evasion

---

##  Recomendaciones
1. Incentivar los **contratos de mayor duración** para fidelizar a los clientes.
2. Fomentar el uso de **pagos automáticos** en lugar de cheques electrónicos, esto ayuda a fidelizar.
3. Ofrecer **beneficios o campañas especiales** a clientes sin pareja o dependientes con el finde evitar evasiones.
4. Mejorar la experiencia de los servicios con mayor churn (fibra óptica, streaming).
5. Implementar **estrategias personalizadas** según perfil de cliente para reducir la evasión.
