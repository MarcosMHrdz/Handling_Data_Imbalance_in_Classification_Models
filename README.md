![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Laboratorio | Manejo del desequilibrio de datos en los modelos de clasificación

Para este laboratorio y en las próximas lecciones, crearemos un modelo sobre el problema de clasificación binaria de abandono de clientes. Utilizará el archivo `files_for_lab/Customer-Churn.csv`.

### Escenario

Trabaja como analista en este proveedor de servicios de Internet. Se le proporcionan datos históricos sobre los clientes de su empresa y sus tendencias de abandono. Su tarea es crear un modelo de aprendizaje automático que ayude a la empresa a identificar a los clientes que tienen más probabilidades de incumplir o abandonar el servicio y, de esta forma, evitar pérdidas de dichos clientes.

### Instrucciones

En este laboratorio, primero analizaremos el grado de desequilibrio en los datos y lo corregiremos utilizando las técnicas que aprendimos en la clase.

Aquí está la lista de pasos a seguir (construir un modelo simple sin equilibrar los datos):

- Importa las bibliotecas y módulos necesarios que necesites.
- Lea esos datos en Python y llame al marco de datos `churnData`.
- Verifique los tipos de datos de todas las columnas de los datos. Verá que la columna `TotalCharges` es de tipo objeto. Convierta esta columna en un tipo numérico utilizando la función `pd.to_numeric`.
- Verificar si hay valores nulos en el marco de datos. Reemplazar los valores nulos.
- Utilice las siguientes funciones: `tenure`, `SeniorCitizen`, `MonthlyCharges` y `TotalCharges`:
  - Escala las características utilizando un normalizador o un escalador estándar.
  - Dividir los datos en un conjunto de entrenamiento y un conjunto de prueba.
  - Ajustar un modelo de regresión logística a los datos de entrenamiento.
  - Verifique la precisión de los datos de prueba.

**Nota**: Hasta el momento no hemos balanceado los datos.

Gestión del desequilibrio en el conjunto de datos

- Verificar el desequilibrio.
- Utilice las estrategias de remuestreo utilizadas en clase para sobremuestrear y reducir el tamaño del muestreo para crear un equilibrio entre las dos clases.
- Cada vez ajuste el modelo y vea cómo es la precisión del modelo.