# Webinar: IA y Machine Learning

## Aplicación de técnicas de Machine Learning para realizar predicciones de capturas de camarón de profundidad en Chile

**Regularización en Regresión Lineal Múltiple: Ridge, LASSO, Elastic Net e Interpretación Bayesiana**

**Autores:** Dr. Carlos Montenegro Silva y Maximiliano Zilleruelo León

Este repositorio contiene el material de la presentación preparada para el webinar sobre técnicas de regularización aplicadas a regresión lineal múltiple y modelación predictiva. La presentación aborda los fundamentos estadísticos de la regularización, su relación con los problemas de sobreajuste y multicolinealidad, y el compromiso entre sesgo y varianza.

Se desarrollan los métodos **Ridge**, **LASSO** y **Elastic Net**, incluyendo sus funciones objetivo, el efecto de los hiperparámetros, la selección de valores de **lambda** y **alpha** mediante validación cruzada y la estimación de los coeficientes de los modelos. También se presenta la interpretación bayesiana de los métodos de regularización.

La parte aplicada utiliza datos de bitácoras de pesca y considera como variable respuesta la **captura por lance**. Se muestran etapas de preparación de los datos, ingeniería de variables, división en conjuntos de entrenamiento y prueba, ajuste de los modelos y comparación de su desempeño predictivo mediante distintas métricas.

## Contenidos principales

- Regresión lineal múltiple y mínimos cuadrados ordinarios
- Sobreajuste y multicolinealidad
- Regularización y compromiso sesgo-varianza
- Regresión Ridge
- LASSO y selección de variables
- Elastic Net
- Validación cruzada
- Selección de hiperparámetros lambda y alpha
- Interpretación bayesiana
- Métricas de desempeño predictivo
- Aplicación a datos pesqueros
- Implementación computacional en R

## Implementación en R

Los modelos son implementados principalmente mediante el paquete **`glmnet`**, utilizando funciones como:

- `glmnet()` — ajuste de modelos regularizados
- `cv.glmnet()` — selección de lambda mediante validación cruzada
- `coef()` — extracción de coeficientes
- `predict()` — generación de predicciones
- `plot()` — visualización de resultados del ajuste

En `glmnet`, el parámetro `alpha` permite especificar:

- `alpha = 0` → Ridge
- `alpha = 1` → LASSO
- `0 < alpha < 1` → Elastic Net

## Archivos

El repositorio contiene la presentación y los materiales asociados al webinar.

## Uso

Este material se comparte con fines académicos, docentes y de divulgación. Si se utiliza o adapta parte del contenido, se agradece citar a los autores y este repositorio.
