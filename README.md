# TelecomX LATAM — Análisis de Evasión de Clientes (Churn)

Análisis exploratorio y estratégico del churn de clientes de TelecomX, identificando los factores clave que llevan a la cancelación del servicio y cuantificando su impacto financiero.

---

## Estructura del proyecto

```
├── TelecomX_Churn_Analysis_Final.ipynb   # Notebook principal
├── requirements.txt                       # Dependencias
└── README.md                              # Este archivo
```

---

## Cómo ejecutar

**1. Clonar o descargar el repositorio**

```bash
git clone <url-del-repo>
cd telecomx-churn
```

**2. Instalar dependencias**

```bash
pip install -r requirements.txt
```

**3. Abrir el notebook**

```bash
jupyter notebook TelecomX_Churn_Analysis_Final.ipynb
```

> También puede abrirse directamente en **Google Colab** sin instalación local.

---

## Contenido del notebook

| Sección | Descripción |
|---|---|
| Extracción | Carga del dataset JSON desde la API de GitHub |
| Transformación | Limpieza, normalización, ingeniería de características y traducción al español |
| Análisis Exploratorio | Visualización de la evasión por contrato, pago, internet, perfil demográfico y variables numéricas |
| Análisis Avanzado | Mapa de correlaciones, escudo de retención, brecha digital, ancla familiar y prueba de hipótesis |
| Impacto Financiero | Cuantificación mensual de ingresos perdidos por evasión |
| Conclusiones | Tabla de factores de riesgo y recomendaciones estratégicas accionables |

---

## Principales hallazgos

- **Tasa de evasión global: ~26%**, representando más de **$139,000 USD perdidos al mes** (~30% de la facturación potencial).
- Los clientes con **contrato mes a mes** evaden ~4× más que los de contratos anuales o bianuales.
- El **cheque electrónico** (pago manual) predice evasión: ~45% vs ~15% en pagos automáticos.
- La **fibra óptica sin soporte técnico** duplica la tasa de evasión respecto a fibra con soporte.
- Los **adultos mayores forzados a facturación digital** presentan las tasas de abandono más altas.
- Cada servicio extra contratado (seguridad, backup, soporte, protección) actúa como un **"ancla" de retención**.

---

## Fuente de datos

**Dataset:** [TelecomX LATAM — Alura Cursos](https://raw.githubusercontent.com/alura-cursos/challenge2-data-science-LATAM/refs/heads/main/TelecomX_Data.json)

El dataset contiene información de ~7,000 clientes con variables demográficas, de servicios contratados y de facturación.

---

## Tecnologías utilizadas

- **Python 3.10+**
- `pandas` — manipulación y transformación de datos
- `numpy` — operaciones numéricas
- `matplotlib` + `seaborn` — visualizaciones
- `requests` — carga de datos desde API

---

## Licencia

Proyecto educativo desarrollado como parte del **Challenge 2 de Data Science — Alura LATAM**.
