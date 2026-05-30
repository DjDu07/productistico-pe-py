# ProductísticoPE - Producción Agrícola en el Perú 🇵🇪

**ProductísticoPE** es una aplicación web interactiva desarrollada para el análisis estadístico y la visualización de la producción y exportación de cultivos en diversas regiones del Perú. Basada en datos del INEI, la plataforma transforma datos tabulares crudos en información estratégica para la toma de decisiones en el sector agrícola.

## Requisitos del Sistema Cumplidos
De acuerdo con la especificación técnica del proyecto, el sistema cumple con:
- **Carga y Gestión de Datos:** Lectura e integración de archivos estructurados en formatos CSV (`Tabla1.csv`) y Excel (`Tabla2.xlsx`).
- **Procesamiento Estadístico:** Cálculo automatizado de medidas de tendencia central (media, mediana, moda) y dispersión (varianza, desviación estándar, rango intercuartílico).
- **Modelado Predictivo:** Análisis de relaciones mediante el coeficiente de correlación de Pearson y covarianza, además del desarrollo de un modelo de Regresión Lineal Simple para predecir la producción basada en el área cosechada.

## Visualizaciones e Interfaz Interactiva
La aplicación utiliza **Streamlit** para desplegar un menú de selección que renderiza:
- **Gráficos de Líneas:** Tendencias de producción de maíz y papa entre años seleccionados.
- **Gráficos de Barras Comparativos:** Comparación de exportaciones y producción de arroz por regiones.
- **Gráficos de Dispersión e Histogramas:** Relación de área cosechada/producción y análisis distribucional de frecuencias.
- **Gráficos de Pastel:** Distribución porcentual de la producción regional anual.
- **Módulo de Exportación:** Permite guardar la información procesada de regreso a formatos CSV o Excel.

## Arquitectura y Tecnologías
El proyecto se diseñó bajo el paradigma de Programación Orientada a Objetos (POO) mediante la clase principal `AgriculturaData` y las siguientes librerías especializadas:
- **Pandas & NumPy:** Manipulación, limpieza y soporte de arreglos matriciales numéricos.
- **Matplotlib & Seaborn:** Construcción y personalización estética de gráficos estadísticos.
- **Scikit-Learn (Sklearn):** Implementación del motor de Regresión Lineal para analítica predictiva.
- **Streamlit:** Framework principal para el despliegue de la interfaz de usuario interactiva.

## Instalación y Uso
1. Tener los archivos `Tabla1.csv` y `Tabla2.xlsx` en la raíz del directorio.
2. Instalar las dependencias necesarias:
   ```bash
   pip install pandas streamlit matplotlib numpy scikit-learn openpyxl seaborn
   ```
3. Ejecutar el entorno interactivo desde la terminal:
   ```bash
   python -m streamlit run app.py
   ```

## 👥 Créditos y Autoría
Este proyecto fue desarrollado de forma grupal como parte del curso Programación Orientada a Objetos en la UPC. Integrantes: Diego Joaquín Díaz Urday, Diego Alberto Aquino Chaccara y Manuel Jesus Chavez Cuba.
