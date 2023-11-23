# Análisis de calidad de vinos

El conjunto de datos esta disponible en UCI machine learning repository, https://archive.ics.uci.edu/ml/datasets/wine+quality

Para más detalles consultar [Cortez et al., 2009]. 

Cita: Cortez,Paulo, Cerdeira,A., Almeida,F., Matos,T., and Reis,J.. (2009). Wine Quality. UCI Machine Learning Repository. https://doi.org/10.24432/C56S3T.

Se utilizaron algoritmos de machine learning para predecir la calidad de vinos. El mejor modelo de clasificación fue XGBoostClassifier, con una exactitud promedio de 63%. Se obtuvo una exactitud baja debido a que había un desbalance entre las clases de la variable calidad.

También, debido al desbalance entre las clases de la variable calidad el modelo predice con mayor frecuencia a las clases 5, 6 y 7. Lo cual hace que estas clases tengan mucho recall y poca precisión.

 Utilizando el modelo XGBRegressor con una tolerancia de 1.0 se obtiene una exactitud de 86.47%.

 La exactitud de los modelos de clasificación puede mejorar aplicando un tratamiento de clases desbalanceadas como: sobremuestreo o el algoritmo SMOTE.
