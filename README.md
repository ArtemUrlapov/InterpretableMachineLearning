# Interpretable Machine Learning - Sistema Experto para Predicción y Mejora del Rendimiento Escolar
## Artem Urlapov Sedova

<p align="justify">
  
En el presente trabajo, buscamos predecir y mejorar el rendimiento de los alumnos de dos colegios desaventajados.
  
Así, tenemos una serie de variables estructurales (caso del rendimiento -promedio en lo académico- del primer período, del segundo período o el -bajo- nivel educativo de los padres) a la vez que otras variables coyunturales (ausencias a clase o consumo de alcohol). Consecuentemente, en el Sistema Experto buscamos incidir sobre las variables coyunturales. Así, creemos poder mejorar nuestra variable objetivo (nota final) reduciendo las ausencias a clase y el consumo de alcohol entre semana. Dejamos como ambiguo el potencial efecto de otras dos variables: tiempo libre y consumo de alcohol entre semana.

A fin de captar mejor las posibles no linealidades, recurrimos al método de Spearman en el análisis de correlaciones y utilizamos Principal Component Analysis como técnica de preprocesamiento de datos.

Hacemos uso de dos algoritmos de Supervised Machine Learning (Stochastic Gradient Boosting, con un MSE alcanzado de 0.16 y Random Forest, con un MSE obtenido de 0.15), cuyos resultados contrastamos a su vez mediante los algoritmos de Interpretable Machine Learning LIME y SHAP. 

Finalmente, probamos obtener un ajuste aún mejor mediante las técnicas de Deep Learning de las Redes Neuronales Artificiales y Long-Short Term Memory, si bien no consiguen superar los resultados de las dos algoritmos de Machine Learning previamente mencionados (en parte, debido al hecho de que se trata de un dataset relativamente pequeño).

Los resultados nos muestran que la variable ausencias a clase es clave para mejorar el rendimiento escolar. El método SHAP (presentado como más robusto que LIME), concretamente, nos sugiere otorgar una mayor ponderación a esta variable. Por otra parte, el efecto de las otras tres variables coyunturales (consumo de alcohol entre semana, consumo de alcohol los fines de semana y tiempo libre) es marginal.

</p>
