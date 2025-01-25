# Proyecto de Análisis de Churn Amazon Prime

<div style="text-align: center;">
     <img src="IMG/PortadaAmazonChurn.webp"
     alt="dashboard /">
</div>

Este proyecto tiene como objetivo analizar la tasa de abandono (churn) de clientes Amazon Prime, utilizando datos históricos y mostrando los resultados en un dashboard interactivo.

## Descripción del Proyecto

El análisis de churn busca identificar patrones y factores que contribuyen al abandono de clientes.
El resultado final de este proyecto es un dasboard que permite visualizar métricas calve, análisis descriptivos y gráficos interactivos para comprender mejor el comportamiento de los clientes.

## Estructura del Proyecto

```bash
Analisis_Amazon/

|---Data/      #Carpeta con los archivos utilizados
|  |
|  |---Data_Analisis/    #Carpeta con los archivos utilizados para analizar los datos
|  |
|  |  |---amazon_churn_analisis_descriptivo.xlsx
|  |  |---Analisis_descriptivo_cat_temp_churn.xlsx
|  |  |___Analisis_descriptivo_num_churn.xlsx
|  |
|  |---Data_Dashboard/        #Carpeta con el dashboard final
|  |
|  |  |___Dashboard.xlsx
|  |
|  |---Data_raw/        #Carpeta con los archivos originales
|  |
|  |  |___amazon_churn_datosbrutos.xlsx
|  |
|  |---Data_transformacion/        #Carpeta con los datos transformados antes de su análisis
|  |
|  |  |___amazon_churn_transformacion.xlsx
|  |
|---IMG/       #Carpeta con imágenes utilizadas en el README.md
|  |
|  |---PortadaAmazonChurn.webp
|  |---DashboardAmazonChurn.png
|  |
|---Recap de sesiones/        #Carpeta con los documentos de recap de cada sesión
|  |
|  |---Recap primera sesion.docx
|  |---Recap segunda sesion.docx
|  |---Recap tercera sesion.docx
|  |---Recap cuarta sesion.docx
|  |---Recap quinta sesion.docx
|  |---Recap sexta sesion.docx
|  |___Recap septima sesion.docx
|  |
|___README.md
```

## Estructura de Datos

El archivo de datos original consta de varias columnas

- **CustomerID**: Identificador único de cada cliente.
- **Churn Label**: Etiqueta que indica si el cliente se fue (Yes ) o no (No).
- **Churned**: Variable binaria (0 o 1) que indica si el cietne abandonó el servicio (1) o se mantuvo (0).
- **Account Length (in months)**: Tiempo que el cliente ha estado suscrito al servicio, en meses.
- **Customer Service Calls**: Número de llamadas realizadas al servicio de atención al cliente.
- **Avg. Monthly GB Download**: Promedio mensual de datos descargados por el cliente en GB
- **Unlimited Data Plan**: Indica si el cliente tiene un plan de datos ilimitado (1: Sì , 0:No)
- **Extra Data Charges**: Cargos adicionales por uso de datos más allá del límite del plan.
- **State**: Estado de residencia del cliente.
- **Phone Number**: Número de teléfono del cliente.
- **Gender**: Género del cliente.
  **Age**: Edad del cliente.
- **Under 30**: Indica si el cliente es menor de 30 años (1: Sì , 0:No).
- **Senior**: Indica si el cliente es mayor de 65 años (1: Sì , 0:No).
- **Group**: Indica si el cliente tiene contratado un plan familiar.
- **Number of Customers in Group**: Número de clientes que pertenecen al mismo plan familiar.
- **Device Protection & Online Backup**: Indica si el cliente tiene protección de dispositivo y respaldo en línea.
- **Contract Type**: Tipo de contrato(Mensual, anual, etc.).
- **Payment Method**: Método de pago utilizado por el cliente.
- **Monthly Charges**: Cargo mensual que el cliente paga por el servicio.
- **Total Charges**: Cargos totales acumulados durante la suscripción.
- **Churn Category**: Categoría que indica el motivo de la deserción (churn).
- **Churn Reason**: Razón específica por la que el cliente abandonó el servicio.
- **Contact Date**: Fecha del último contacto con el cliente.
- **Last Transaction Date**: Fecha de la última transacción realizada por el cliente.
- **Tenure(in months)**: Tiempo total de suscripción del cliente.
- **Customer Segment**: Clasificación del cliente según su nivel de uso o importancia (Alto, Medio, Bajo).
- **Average Monthly Expenses**: Gasto promedio mensual del cliente
- **Number of Complaints of support**: Número de quejas o interacciones con el servicio de soporte
- **Preferec Contact Method**: Método preferido por el cliente para ser contactado (email teléfono,etc.).
- **Applied Discount**: Indica si se ha aplicado algún descuento al cliente.
- **Hobby**: Pasatiempos del cliente.
- **Favorite TV Show**: Programa de televisión favorito del cliente.
- **Internal Notes**: Notas internas relacionadas con el cliente.

## Desarrollo del proyecto

### Primera sesion

- Entendimiento general del conjunto de datos y de las columnas.

### Segunda sesion

- Eliminación de columnas, establecimiento del tipo de los datos y normalización de datos.

### Tercera sesion

- Análisis descriptivo de las columnas numéricas

### Cuarta sesion

- Análisis descriptivo de las columnas categóricas y temporales.

### Quinta sesion

- Análisis descriptivos de las columnas numéricas junto con la columna objetivo.

### Sexta sesion

- Análisis descriptivos de las columnas categòricas y temporales junto con la columna objetivo.
- Creacion de nuevas columnas.

### Septima sesion

- Elección de las columnas relevantes para el Dashboard.

### Octava sesion

- Creación del Dashboard final

## Dashboard

<div style="text-align: center;">
     <img src="IMG/DashboardAmazonChurn.png" alt="dashboard /">
</div>

## Conclusiones

- Tenemos una tasa de abandono del 27%
- El gasto promedio de las personas que abandonan el servicio, es un 6% superior a la media de gasto mensual, mientras que para las personas que siguen en la plataforma es de un 2% inferior.
- La principal razon de este abandono es una mejor oferta de la competencia
- Hemos observado como al aumentar el número de llamadas al servicio de atención al cliente, aumenta el porcentaje de abandono del servicio
- Los contratos de larga duracion(un año / dos años) tienen un efecto beneficioso, ya que disminuye drasticamente la tasa de abandono
- El abandono está estrechamente relacionado con el método de pago (aumentando en el caso de débito y tarjetas) y con las multicuentas (aumentando en el caso de cuentas individuales)

## Contribuciones

Las contribuciones a este proyecto son muy bienvenidas. Si tienes alguna sugerencia, mejora o corrección, no dudes en ponerte en contacto o enviar tus ideas.

## Autores

- Mª Cruz - [Github Profile](https://github.com/MariCruzTE)

**Con la inestimable guia y consejos de**:

- Jaime thePower- [Github Profile](https://github.com/RCJaime)

- Silvia thePower - [Github Profile](https://github.com/Salsi95)
