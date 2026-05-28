# ProductísticoPE - Producción Agrícola en el Perú 🇵🇪

**ProductísticoPE** es una aplicación web interactiva desarrollada para el análisis estadístico y la visualización de la producción y exportación de cultivos en diversas regiones del Perú. Basada en datos del INEI, la plataforma transforma datos tabulares crudos en información estratégica para la toma de decisiones en el sector agrícola [cite: 42, 176].

## Requisitos del Sistema Cumplidos
De acuerdo con la especificación técnica del proyecto, el sistema cumple con:
- **Carga y Gestión de Datos:** Lectura e integración de archivos estructurados en formatos CSV (`Tabla1.csv`) y Excel (`Tabla2.xlsx`) [cite: 175, 183].
- **Procesamiento Estadístico:** Cálculo automatizado de medidas de tendencia central (media, mediana, moda) y dispersión (varianza, desviación estándar, rango intercuartílico) [cite: 183].
- **Modelado Predictivo:** Análisis de relaciones mediante el coeficiente de correlación de Pearson y covarianza, además del desarrollo de un modelo de Regresión Lineal Simple para predecir la producción basada en el área cosechada [cite: 183].

## Visualizaciones e Interfaz Interactiva
La aplicación utiliza **Streamlit** para desplegar un menú de selección que renderiza [cite: 183, 186]:
- **Gráficos de Líneas:** Tendencias de producción de maíz y papa entre años seleccionados [cite: 12, 183].
- **Gráficos de Barras Comparativos:** Comparación de exportaciones y producción de arroz por regiones [cite: 183].
- **Gráficos de Dispersión e Histogramas:** Relación de área cosechada/producción y análisis distribucional de frecuencias [cite: 183].
- **Gráficos de Pastel:** Distribución porcentual de la producción regional anual [cite: 12, 183].
- **Módulo de Exportación:** Permite guardar la información procesada de regreso a formatos CSV o Excel [cite: 183].

## Arquitectura y Tecnologías
El proyecto se diseñó bajo el paradigma de Programación Orientada a Objetos mediante la clase principal `AgriculturaData` y las siguientes librerías especializadas [cite: 2, 181]:
- **Pandas & NumPy:** Manipulación, limpieza y soporte de arreglos matriciales numéricos [cite: 133, 164, 183].
- **Matplotlib & Seaborn:** Construcción y personalización estética de gráficos estadísticos [cite: 146, 154].
- **Scikit-Learn (Sklearn):** Implementación del motor de Regresión Lineal para analítica predictiva [cite: 23, 183].
- **Streamlit:** Framework principal para el despliegue de la interfaz de usuario interactiva[cite: 137, 183].

## Instalación y Uso
1. Asegúrate de tener los archivos `Tabla1.csv` y `Tabla2.xlsx` en la raíz del directorio[cite: 175].
2. Instala las dependencias necesarias:
   ```bash
   pip install pandas streamlit matplotlib numpy scikit-learn openpyxl seaborn
   ```
3. Ejecuta el entorno interactivo desde tu terminal:
   ```bash
   python -m streamlit run app.py
   ```
