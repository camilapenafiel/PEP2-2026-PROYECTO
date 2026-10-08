# UNICLIMA METRICS

## Descripción

UNICLIMA METRICS es un proyecto IoT orientado a medir y visualizar condiciones climáticas locales en el campus de UNIFRANZ.

El sistema contempla una estación meteorológica de bajo costo basada en ESP32 y sensores para obtener temperatura, humedad relativa, presión barométrica, precipitación y radiación UV. Los datos serán comunicados mediante HTTP, almacenados en SQL Server y utilizados para visualización, análisis, alertas y reportes históricos.

## Objetivo

Implementar una estación meteorológica IoT automatizada que permita recopilar datos climáticos locales, almacenarlos en una base de datos SQL Server, analizarlos mediante reglas definidas en el proyecto y presentarlos mediante una interfaz amigable.

## Tecnologías y componentes previstos

- ESP32
- BMP280
- DHT11
- FC-37
- Sensor de radiación UV
- Comunicación Wi-Fi mediante HTTP
- SQL Server
- C++
- C#
- Interfaz gráfica / aplicación
- Reportes en PDF y Excel

## Funcionalidades principales

- Monitoreo de temperatura, humedad, presión, precipitación y UV.
- Visualización dinámica del estado climático.
- Alertas relacionadas con índice UV y variaciones de presión.
- Cálculo de un índice acumulativo de sequía.
- Administración de estaciones y acceso por roles.
- Consulta histórica por rango de fechas.
- Exportación de reportes a PDF y Excel.

## Organización del repositorio

```text
PEP2-2026-PROYECTO/
├── README.md
├── docs/
│   ├── proyecto/
│   ├── presentacion/
│   ├── planificacion/
│   ├── requisitos/
│   ├── analisis/
│   └── tecnica/
│       ├── arquitectura/
│       ├── base-datos/
│       ├── hardware/
│       ├── uml/
│       └── interfaz/
├── src/
│   ├── esp32/
│   └── aplicacion/
│       ├── presentacion/
│       ├── negocio/
│       └── datos/
├── database/
│   ├── scripts/
│   └── consultas/
├── tests/
│   ├── hardware/
│   ├── software/
│   └── integracion/
├── resources/
│   ├── images/
│   └── diagrams/
├── EQUIPO/
└── .github/
    └── ISSUE_TEMPLATE/
```

## Metodología

El proyecto seguirá Scrum, con actividades de refinamiento, planificación de Sprint, construcción, revisión y retrospectiva.

## Hitos

- **Hito 2:** definición y alcance.
- **Hito 3:** primer prototipo funcional.
- **Hito 4:** sistema al 90%.
- **Hito 5:** sistema final al 100%.

## Alcance actual

El repositorio servirá como centro de control del proyecto durante el semestre. En él se organizarán la documentación, planificación, requisitos, diagramas, código, scripts de base de datos, pruebas, recursos y evidencias del desarrollo.

> Nota: la documentación del proyecto debe mantenerse alineada con el informe académico vigente. La definición final de la tecnología de la aplicación deberá aclararse posteriormente, ya que el informe menciona tanto una aplicación web como Windows Forms/C#.
