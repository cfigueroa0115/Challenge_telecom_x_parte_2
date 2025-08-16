# Challenge_telecom_x_parte_2

# Predicción de Cancelación de Clientes – Telecom X

## Resumen del proyecto
El propósito de este proyecto es construir modelos de Machine Learning que permitan predecir si un cliente de Telecom X tiene probabilidad de cancelar su servicio (**Churn**). Detectar estos clientes a tiempo ayuda a diseñar estrategias de retención y mejorar la lealtad del cliente.

El análisis contempla:
- Preparación y depuración de los datos.
- Conversión de variables categóricas a formato numérico.
- Exploración y visualización de datos.
- Creación y evaluación de modelos predictivos.
- Determinación de las características más relevantes que influyen en la cancelación.

## Datos
El conjunto de datos incluye información histórica de clientes, como:
- Características demográficas (edad, género, estado civil, etc.).
- Detalles de los contratos y servicios contratados.
- Cargos y consumos (`TotalCharges`, `DailyCharges`).
- Etiqueta de salida: `Churn` (1 = canceló, 0 = activo).

> Nota: Antes de modelar, los datos fueron limpiados, se manejaron valores faltantes y se codificaron las variables categóricas.

## Herramientas y librerías
- **Python 3.x**
- **pandas** y **numpy** para manipulación de datos.
- **matplotlib** y **seaborn** para gráficos y visualización.
- **scikit-learn** para el modelado:
  - Random Forest
  - Regresión Logística
  - Preprocesamiento: StandardScaler, SimpleImputer, train_test_split
- **Jupyter Notebook / Google Colab** para la ejecución del proyecto.


## Metodología
1. **Carga y limpieza:** se eliminaron columnas innecesarias y se trataron valores faltantes.  
2. **Codificación:** se aplicó one-hot encoding y se transformaron booleanos a enteros.  
3. **Exploración:** se analizaron distribuciones, boxplots y matriz de correlación.  
4. **Preparación para modelado:** división de datos en entrenamiento y prueba; normalización de variables donde se requiere.  
5. **Modelado:** se entrenaron Random Forest y Regresión Logística.  
6. **Evaluación:** se calcularon métricas como exactitud, precisión, recall, F1-score y matriz de confusión.  
7. **Análisis de variables importantes:** se identificaron los factores que más influyen en la cancelación.  
8. **Conclusiones y recomendaciones:** propuestas de retención basadas en el análisis.

## Resultados principales
- Rendimiento de los modelos: ~78-79% de exactitud.  
- Factores que más impactan la cancelación: `Tenure`, `TotalCharges`, `Contract`, `NumServicios`, `PaymentMethod`.  
- Recomendaciones estratégicas:
  - Fomentar contratos de mayor duración.  
  - Implementar seguimiento y programas de bienvenida para clientes recientes.  
  - Incentivar pagos automáticos.  
  - Proporcionar soporte proactivo a clientes de fibra óptica.  
  - Diseñar paquetes personalizados para clientes con alto gasto.

## Instrucciones para ejecutar
1. Clonar el repositorio:
```bash
git clone https://github.com/usuario/telecom-x-churn.git

