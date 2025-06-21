# 📊 Evaluador de Proyectos de Inversión con Python

Este repositorio surge como una herramienta práctica para ayudar a **inversionistas promisorio/as** sin la necesidad de tener una alta expertiz financiera o técnica a evaluar proyectos con fundamentos sólidos y simulaciones claras.

El objetivo es entregar **una guía accesible** para responder preguntas clave como:

- ¿Es buena idea invertir en este proyecto?
- ¿En cuánto tiempo recuperaré la inversión?
- ¿Qué tan riesgoso es el peor escenario?
- ¿Cuáles son mis probabilidades reales de tener ganancias?

---

## 🔍 Motivación

En muchas decisiones de inversión, especialmente en PyMEs o negocios emergentes, el análisis financiero se reduce a intuición o Excel básicos.
Este proyecto busca entregar **tres niveles de análisis financiero progresivos**, todos en Python, con un foco práctico pero con métricas clásicas: **VAN, TIR, Payback** y algunas más avanzadas: **VaR, Expected Shortfall** junto con visualizaciones útiles para tomar de decisiones.

---

## 📁 Estructura del Proyecto

### 1️⃣ `Codigo_Evaluacion_Simple.ipynb`

🔹 **Propósito**: evaluación tradicional con un único escenario de crecimiento proyectado.

🔹 **Métricas calculadas**:
- VAN
- TIR
- Payback

🔹 **Ideal para**: una estimación preliminar, rápida y sin considerar incertidumbre.

---

### 2️⃣ `Codigo_Evaluacion_Multiescenario.ipynb`

🔹 **Propósito**: evaluar un proyecto bajo múltiples escenarios en virtud de distintas tasas de crecimiento, que se determinan constante.

🔹 **Métricas calculadas**:
- VAN
- TIR
- Payback (por cada escenario)

🔹 **Visualizaciones**:
- VAN y TIR según la tasa de crecimiento 📈

⚠️ *Importante*: aquí no se usan histogramas, porque **cada escenario depende del anterior** y no es estadísticamente correcto tratarlos como independientes.

---

### 3️⃣ `Codigo_Evaluacion_Estocastico.ipynb`

🔹 **Propósito**: evaluación probabilística mediante simulaciones independientes (**cuasi Monte Carlo**), incorporando incertidumbre mensual en ingresos, costos, demanda y gastos.

🔹 **Métricas calculadas**:
- VAN
- TIR
- Payback
- Value at Risk (VaR 95%)
- Expected Shortfall (ES 95%)

🔹 **Visualizaciones**:
- Histogramas y boxplots de VAN, TIR y Payback
- Violin plots para explorar la distribución y densidad de los escenarios

✅ Este es el análisis más completo y realista del proyecto.

---

## 🧠 ¿Qué se puede hacer con este repositorio?

✔️ Estimar en cuánto tiempo recuperarás tu inversión
✔️ Medir la rentabilidad esperada bajo incertidumbre
✔️ Visualizar qué tan probable es que el proyecto sea rentable
✔️ Medir el riesgo extremo de perder dinero (VaR y ES)
✔️ Ajustar decisiones según tu tolerancia al riesgo

---

## 🚀 Requisitos

- Python 3.10+
- Jupyter Notebook
- numpy
- pandas
- numpy-financial
- matplotlib
- seaborn

Instalar dependencias:

```bash
pip install numpy pandas numpy-financial matplotlib seaborn

## 🤝 Contribuciones

¿Quieres mejorar este repositorio o adaptarlo a otros tipos de inversión? ¡Bienvenido! Puedes enviar un PR o abrir un issue.

[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/tu-usuario/evaluador-proyectos/issues)
