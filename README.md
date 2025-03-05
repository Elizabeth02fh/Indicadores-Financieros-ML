📊 Análisis de Indicadores Financieros con Machine Learning

📌 Descripción del Proyecto

Big Finance S. A. es una empresa dedicada al sector bancario, especializada en la concesión de préstamos a empresas. Actualmente, la empresa mantiene relaciones comerciales con 3,932 clientes y busca mejorar su análisis de riesgos financieros.

En este proyecto, se ha desarrollado un modelo de Machine Learning para analizar indicadores financieros y predecir la clasificación de riesgo (Rating) de los clientes con base en la base de datos credittable.xls.

Los principales objetivos del análisis son:

📌 Modelo de regresión: Predecir una variable de interés en función de otras.

📌 Modelo de clasificación: Predecir el Rating de un cliente según los indicadores financieros.

📌 Evaluación del desempeño de los modelos: Usar métricas como R², matriz de confusión y otras medidas de bondad de ajuste.

📌 Predicción del Rating de un nuevo cliente con base en el modelo de clasificación elegido.

🚀 Tecnologías Utilizadas

Python 🐍

Librerías: pandas, numpy, scikit-learn, XGBoost, matplotlib, seaborn

Modelos utilizados: Regresión Logística, Random Forest, SVC, XGBoost

📊 ¿Qué muestran estos gráficos?

✅ Comparación de (R²) entre Modelos de Regresión
![image](https://github.com/user-attachments/assets/89b94dbc-b164-4d82-a9a5-f3d4122a02d9)
En el gráfico, se observa que el modelo de regresión Random Forest obtuvo el mayor Coeficiente de Determinación (R² = 91.28%), lo que lo convierte en un modelo altamente predictivo para la variable EBIT_TA. Esto indica que las variables seleccionadas explican de manera efectiva la variabilidad de la rentabilidad operativa sobre activos.

✅ Gráfico de Valores Reales vs. Predichos (Random Forest)
![image](https://github.com/user-attachments/assets/6ecde697-1b95-4383-bd9a-51aac69f8c6d)

En este gráfico:

Puntos azules: Representan las predicciones del modelo.

Línea roja: Indica los valores reales de EBIT_TA.

Los puntos están alineados con la línea roja, lo que indica que el modelo predice con precisión y tiene un buen desempeño al estimar esta variable financiera a partir de WC_TA, RE_TA, MVE_BVTD, S_TA e Industry.

✅ Histograma de errores (Random Forest)
![image](https://github.com/user-attachments/assets/5b06e916-435f-4add-ae6a-b5bd1cc0072b)

El modelo Random Forest tiene un buen desempeño, ya que sus errores están distribuidos de manera equilibrada alrededor de 0, sin valores extremos que sugieran sobreajuste (overfitting) o subajuste (underfitting).

📌 Resumen de la Matriz de Confusión del Modelo SVC
![image](https://github.com/user-attachments/assets/51ae1657-07fc-4999-a655-dbbddb6ef365)

El modelo SVC (Support Vector Classifier) muestra un buen rendimiento, ya que la mayoría de las predicciones están en la diagonal principal, lo que indica una alta precisión en varias clases. Sin embargo, aún hay algunas confusiones, especialmente en la clase "BBB", donde:
✔️ 156 casos fueron correctamente clasificados como "BBB".
❌ 36 casos fueron clasificados incorrectamente en otra categoría.
❌ 16 casos adicionales también fueron mal clasificados.

✅ Comparación de Precisión de Modelos 

![image](https://github.com/user-attachments/assets/97b4b54d-36e2-4595-bb51-0a5637993621)
📌 Precisión del modelo SVC: 73.82%, superando a los demás algoritmos evaluados.

📊 Distribución de Clases en el Dataset
![image](https://github.com/user-attachments/assets/764605df-2f8a-447f-8f30-eb77a6950574)


El histograma de frecuencias muestra que las categorías BBB, BB y AAA tienen la mayor cantidad de datos, lo que indica que estas clases predominan en el conjunto de datos.

📌  Aquí, se muestra una parte de codigo, la Predicción del Rating de un nuevo cliente con base en el modelo de clasificación elegido.
![image](https://github.com/user-attachments/assets/f43d31c3-f084-47ec-9f42-b94b1eece0bd)

🏆 Conclusiones

Random Forest es el mejor modelo de regresión para predecir EBIT_TA.

SVC es el mejor modelo de clasificación, logrando una precisión del 73.82%.

La matriz de confusión indica que la mayoría de las predicciones son correctas, aunque hay algunas confusiones en ciertas clases.

El histograma de errores muestra que Random Forest no tiene problemas de sobreajuste ni subajuste.

🔗 Enlace al Proyecto

📂 Puedes ver el código completo y los análisis en mi repositorio de GitHub: [🔗 https://github.com/Elizabeth02fh]

📌 Si te interesa el Machine Learning en Finanzas, ¡conectemos y conversemos! 🤝🚀
