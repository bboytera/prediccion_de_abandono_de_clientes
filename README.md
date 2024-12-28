# Prediccion_de_abandono_de_clientes
creacion de modelos supervisados, regresion logistica, arbol de desicion, y bosque aleatorio
# Introducción
Los clientes de Beta Bank se están yendo cada mes poco a poco. Los banqueros descubrieron que es más barato salvar a los clientes existentes que atraer nuevos. Necesitamos predecir si un cliente dejará el banco pronto. Contamos con los datos sobre el comportamiento pasado de los clientes y la terminación de contratos con el banco. Crearemos un modelo con el máximo valor F1 posible. Para aprobar la revisión, necesitamos un valor F1 de al menos 0.59. Verificaremos el valor F1 para el conjunto de prueba. Además mediremos la métrica AUC-ROC y compararla con el valor F1.
# Descripción de los datos
Puedes encontrar los datos en el archivo  /datasets/Churn.csv 


 **Características**


- `RowNumber`: índice de cadena de datos
- `CustomerId`: identificador de cliente único
- `Surname`: apellido
- `CreditScore`: valor de crédito
- `Geography`: país de residencia
- `Gender`: sexo
- `Age`: edad
- `Tenure`: período durante el cual ha madurado el depósito a plazo fijo de un cliente (años)
- `Balance`: saldo de la cuenta
- `NumOfProducts`: número de productos bancarios utilizados por el cliente
- `HasCrCard`: el cliente tiene una tarjeta de crédito (1 - sí; 0 - no)
- `IsActiveMember`: actividad del cliente (1 - sí; 0 - no)
- `EstimatedSalary`: salario estimado


 **Objetivo**


- `Exited`: El cliente se ha ido (1 - sí; 0 - no)
# Habilidades técnicas
- Phyton
- Pandas
- Numpy
- Matplotlib
- Scikit-learn
- Métricas de evaluación como precisión, recall, valor F1 y AUC-ROC.
- Ajustar los pesos de clase, el submuestreo, el sobremuestreo.
# Conclusión General
Logramos un **F1-score de 0.5904 y un AUC-ROC de 0.5044** en el conjunto de prueba después de corregir el desequilibrio utilizando **sobremuestreo** (oversampling) con el **modelo de regresion logistica!!**. Esto sugiere que nuestro modelo está realizando una clasificación aceptablemente buena, aunque el AUC-ROC indica un rendimiento algo bajo en la capacidad de distinguir entre clases.
