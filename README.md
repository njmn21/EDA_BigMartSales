# Análisis Exploratorio de Datos (EDA) para BigMart

## 1. Objetivo del Análisis

### Definición del Problema de Negocio
BigMart es una empresa de retail que vende diversos productos en 10 tiendas en diferentes ciudades. Debido al impacto del COVID-19, algunos productos de alta rotación han comenzado a quedarse en el almacén, generando un problema de sobrestock y reduciendo el espacio disponible para otros productos. Esto afecta la capacidad de la empresa para optimizar su inventario y realizar pedidos eficientes a proveedores.

### Objetivo del Análisis
El objetivo es encontrar una manera óptima de gestionar el inventario y mejorar la precisión de los pedidos a proveedores. Para ello, se utilizará el análisis de datos para:

- Identificar patrones de ventas en diferentes productos y tiendas.
- Detectar productos con sobrestock y entender las razones detrás de este fenómeno.
- Predecir la demanda de productos en el futuro inmediato, especialmente para el primer trimestre de 2021 (Q1-2021).
- Optimizar la gestión del inventario, reduciendo el espacio desperdiciado y mejorando la rentabilidad.
- Segmentar tiendas y productos para encontrar diferencias en el comportamiento de ventas según la ubicación y características de la tienda.

### Variables Clave Analizadas
- **Item_Outlet_Sales**: Ventas por producto en cada tienda (métrica clave a analizar).
- **Item_Type**: Categoría del producto (para identificar qué tipos de productos están afectados).
- **Item_Visibility**: Visibilidad del producto en la tienda (para evaluar si la ubicación afecta las ventas).
- **Outlet_Location_Type**: Ubicación de la tienda (para analizar diferencias entre ciudades).
- **Outlet_Size**: Tamaño de la tienda (para entender su impacto en ventas o sobrestock).
- **Item_MRP**: Precio del producto (para examinar si afecta la demanda).

---

## 2. Carga y Comprensión de los Datos
Se cargaron los datos desde el archivo `BigMartSales.csv`. Durante esta etapa se realizó una comprensión inicial de las variables mediante:

- Revisión de las primeras filas del dataset.
- Análisis de las dimensiones del conjunto de datos.
- Verificación de tipos de datos.
- Análisis descriptivo general para identificar posibles anomalías.

---

## 3. Limpieza de Datos
Durante esta etapa, se aplicaron las siguientes acciones:

- Tratamiento de valores nulos en variables categóricas y numéricas.
- Eliminación de registros y/o variables irrelevantes para el análisis.

---

## 4. Análisis Univariado
Este análisis se centró en la distribución y comportamiento de las variables de forma individual, utilizando:

- Histogramas y diagramas de caja para variables numéricas.
- Gráficos de barras para variables categóricas.

---

## 5. Análisis Bivariado
Se analizaron las relaciones entre pares de variables para identificar posibles correlaciones o patrones significativos. Se utilizaron técnicas como:

- Diagramas de dispersión para relaciones entre variables numéricas.
- Diagramas de caja comparativos para analizar ventas por categorías de productos o ubicaciones.

---

## 6. Análisis de Valores Atípicos
Para identificar posibles outliers que afecten el análisis y las predicciones se aplicaron:

- Diagramas de caja y bigotes (Boxplots) para detectar valores extremos.
- Estudio específico en la variable `Item_Outlet_Sales` para entender el impacto de los productos con ventas inusualmente altas o bajas.

---

## Conclusiones
A partir del análisis realizado, se identificaron patrones relevantes relacionados con el sobrestock de ciertos productos y se encontraron posibles acciones para optimizar la gestión del inventario. Se recomienda implementar modelos predictivos para pronosticar la demanda futura y ajustar las órdenes a proveedores de manera más eficiente.

