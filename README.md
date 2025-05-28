# modelo-prediccion-diabetes
# 🧬 Análisis de Defunciones por Diabetes Mellitus
![image](https://github.com/user-attachments/assets/87d4fe82-6aec-4996-90d9-3588096d7958)

Este proyecto corresponde al análisis de datos realizado como parte del diplomado de análisis de datos de ROMAC. Se enfoca en estudiar las defunciones por **diabetes mellitus** en México, identificando patrones, diferencias entre géneros, correlaciones entre variables sociodemográficas y comportamientos mensuales o anuales.

## 📊 Objetivos

- Analizar características clave de las defunciones por diabetes mellitus.
- Identificar diferencias por sexo, edad, escolaridad y ocupación.
- Observar variaciones temporales mensuales y anuales.
- Entrenar modelos predictivos simples para inferir riesgo de muerte por diabetes.
- Visualizar patrones que podrían vincularse con factores sociales o eventos externos como la pandemia por COVID-19.

## 🧾 Conjunto de Datos

El análisis se basó en un dataset de defunciones con atributos como:

- `EDAD`: Edad de la persona fallecida.
- `SEXO`: Género (Hombre / Mujer).
- `ESCOLARIDA`: Nivel de escolaridad.
- `OCUPACION`: Ocupación registrada.
- `ASIST_MEDI`: Asistencia médica recibida.
- `ENTIDAD`: Estado de la república.
- `FECHA_DEF`: Fecha de defunción.
- `CAUSA_DEF`: Descripción médica del motivo de muerte.
- `DEFUN_DIAB`: Variable binaria indicando si fue una muerte por diabetes mellitus.

## 📈 Análisis Exploratorio

Se realizaron las siguientes visualizaciones:

- 📌 Distribución de edad por género.
- 📌 Defunciones por mes.
- 📌 Estado con más muertes (CDMX destacó como el más alto).
- 📌 Comparación anual de muertes (destacando 2020 como un pico por la pandemia).
- 📌 Matriz de correlación de características clave.

## 🧠 Modelado Predictivo

Se aplicó un modelo de regresión logística para predecir la probabilidad de que una defunción haya sido causada por diabetes, utilizando como variables predictoras:

- `SEXO`
- `EDAD`
- `CAUSA_DEF` (transformada a variables numéricas)

Se evaluó el modelo con la métrica ROC AUC.

## 🧪 Resultados Destacados
![image](https://github.com/user-attachments/assets/cb8f28ce-ee88-4854-857a-05f195af114a)

- La edad promedio de defunción fue entre los 60 y 80 años.
- Hay ligeras diferencias de edad y frecuencia entre hombres y mujeres.
- La Ciudad de México fue la entidad con más defunciones.
- De abril a septiembre de 2020 se observó un aumento notable que puede relacionarse con el impacto de la pandemia.
- El modelo predictivo mostró un alto desempeño (AUC ≈ 1, aunque esto puede requerir revisión por posible sobreajuste o data leakage).

## 🔧 Tecnologías

- Python (Pandas, Matplotlib, Seaborn, Scikit-learn)
- Google Colab / Jupyter Notebook
- Visualización con seaborn y matplotlib

## 🚀 Cómo Ejecutar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/analisis-diabetes-romac.git
   cd analisis-diabetes-romac
   ```
