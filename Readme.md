#  Challenge Alura Store

Proyecto de análisis de datos para ayudar al **Cliente** a decidir **qué tienda conviene vender** y así liberar capital para un nuevo negocio.

---

## Resumen

Analizamos las **4 tiendas** del cliente con el fin de identificar la que **genera menores rendimientos**.  
El criterio de evaluación se basó en cinco indicadores clave extraídos de los históricos de ventas.

| Indicador | ¿Por qué importa? |
|-----------|-------------------|
| **Facturación total** | Mide el volumen general de ingresos. |
| **Categorías más populares** | Muestra la concentración de ventas y posibles nichos exitosos. |
| **Calificación promedio de clientes** | Señal de satisfacción y reputación de la tienda. |
| **Productos más y menos vendidos** | Permite ver qué tan diversificada y estable es la demanda. |
| **Costo promedio de envío** | Impacta directamente en la rentabilidad final. |

Cada indicador se normalizó y se asignó una puntuación de **1 (mejor)** a **4 (peor)**; la suma dio un **puntaje global**: a mayor puntaje, menor desempeño.

---

##  Estructura de los datos

Cada tienda dispone de un CSV con las siguientes columnas (obtenidas con `head()`):

| Columna | Descripción |
|---------|-------------|
| `Producto` | Nombre del artículo vendido |
| `Categoría del producto` | Línea/división comercial |
| `Precio` | Valor unitario (COP) |
| `Costo del envío` | Cargo logístico aplicado |
| `Fecha de compra` | YYYY‑MM‑DD |
| `Vendedor` | ID o nombre del vendedor interno |
| `Lugar de compra` | Ciudad del cliente |
| `Calificación` | Puntuación dada por el cliente (1‑5) |
| `Método de pago` | Tarjeta, efectivo, etc. |
| `Cantidad de cuotas` | Nº de pagos cuando es crédito *(práctica común en Colombia)* |
| `lat`, `lon` | Coordenadas geográficas del cliente (latitud y longitud) |

> ***Nota***: Las columnas `lat` y `lon` se utilizaron para análisis geográfico (mapas de calor).

---

## 🔧 Herramientas

- **Python 3.10+**
- **pandas** – limpieza y transformación de datos  
- **matplotlib** – visualización de resultados

    
