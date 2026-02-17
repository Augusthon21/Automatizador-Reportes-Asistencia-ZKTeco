# 📊 Automatizador de Reportes de Asistencia

Esta aplicación web, desarrollada con **Streamlit**, está diseñada para transformar registros biométricos crudos (archivos `.dat`) en reportes de asistencia consolidados, precisos y listos para la toma de decisiones. 
El archivo .dat es extraido de un aparato de registro biométrico ZKTeco
El sistema automatiza el preprocesamiento, la clasificación por turnos, el redondeo de horarios y el cálculo de horas trabajadas, exportando un archivo Excel con formato profesional.

## 🚀 Funcionalidades Principales

- **Ingesta de Datos:** Carga y lectura automática de archivos `.dat` y `.txt`.
- **Clasificación Inteligente:** Separa las marcaciones en ventanas de tiempo (Entrada/Salida Mañana y Entrada/Salida Tarde).
- **Lógica de Redondeo:** Aplica umbrales de tolerancia (ej: 09:01) para determinar puntualidad o tardanzas de forma automática.
- **Imputación de Vacíos:** Completa registros faltantes con horarios estándar basados en el día de la semana (Lunes-Viernes y Sábados).
- **Cálculo de Métricas:** Genera totales de horas trabajadas tanto en formato decimal como en HH:MM:SS.
- **Reporte Estilizado:** Exporta a Excel utilizando `openpyxl` para aplicar colores por categorías, bordes, formatos de fecha/hora y ajuste automático de columnas.
- **Auditoría:** Incluye una columna de "registros brutos" para verificar todas las marcaciones originales del usuario en un día determinado.

## 🛠️ Tecnologías Utilizadas

- **Python 3.x**
- **Streamlit:** Interfaz de usuario web.
- **Pandas:** Procesamiento y limpieza de datos.
- **NumPy:** Lógica condicional vectorizada.
- **Openpyxl:** Estilización y generación de archivos Excel.

## 📦 Instalación y Uso Local

Si deseas ejecutar el proyecto en tu máquina local, sigue estos pasos:

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/Automatizador-Reportes-Asistencia.git](https://github.com/tu-usuario/Automatizador-Reportes-Asistencia.git)
   cd Automatizador-Reportes-Asistencia
