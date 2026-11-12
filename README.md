# RetailPro: Pipeline Analítico y Modelo de Datos

<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-16-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL 16">
  <img src="https://img.shields.io/badge/Power_BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
  <img src="https://img.shields.io/badge/Status-En_Desarrollo-green?style=for-the-badge" alt="Status">
</p>

## 🚀 Descripción del Proyecto

**RetailPro** es una solución integral de ingeniería y análisis de datos diseñada para procesar, transformar y exponer métricas clave de negocio del sector retail. El pipeline centraliza transacciones y dimensiones operativas en una base de datos relacional optimizada en **PostgreSQL 16**, sirviendo como fuente de verdad para un modelo dimensional en **Power BI** estructurado en esquema de estrella (*star-schema*).

---

## 🏗️ Arquitectura y Flujo de Datos

El flujo del dato comprende las siguientes capas:

1. **Ingestión y Almacenamiento (PostgreSQL 16):** Normalización de fuentes transaccionales, aplicación de restricciones de integridad, índices optimizados y consultas avanzadas (`JOINs`, CTEs, funciones de ventana).
2. **Modelado Analítico (Power BI Desktop):** Conexión directa/importación estructurada en tablas de hechos y dimensiones, definición de relaciones unidireccionales y desarrollo de medidas DAX para indicadores de rendimiento (KPIs, YTD, crecimiento interanual).

---

## 📂 Estructura del Repositorio

```text
RetailPro/
│
├── sql/                    # Scripts DDL, DML y consultas de transformación
│   ├── 01_ddl_schema.sql   # Creación de tablas, constraints y tipos
│   ├── 02_seed_data.sql    # Datos iniciales o de prueba
│   └── 03_queries.sql      # Vistas y consultas analíticas avanzadas
│
├── powerbi/                # Artefactos de inteligencia de negocios
│   ├── RetailPro_Model.pbix# Archivo principal de Power BI
│   └── dax_measures.md     # Documentación de fórmulas DAX clave
│
├── docs/                   # Diagramas ER y documentación de arquitectura
│   └── er_diagram.png      # Esquema relacional de la base de datos
│
└── README.md
