# UNICLIMA METRICS

## Nombre del proyecto
**UNICLIMA METRICS**

Sistema IoT de monitoreo climático local para el campus de la Universidad Privada Franz Tamayo (UNIFRANZ).

## Problema
Las aplicaciones meteorológicas convencionales pueden presentar datos poco precisos para una ubicación específica cuando utilizan información proveniente de estaciones o satélites alejados.

En el campus de UNIFRANZ existe la necesidad de contar con mediciones climáticas locales de temperatura, humedad, presión barométrica, precipitación y radiación UV, además de información histórica y alertas.

## Propósito
Desarrollar una estación meteorológica IoT de bajo costo que permita obtener información climática directamente del entorno del campus de UNIFRANZ, almacenar los datos y presentarlos de forma clara para facilitar su consulta, análisis y uso didáctico.

## Usuarios
- **Administrador:** administración de estaciones y funciones administrativas.
- **Investigador / Usuario de Consulta:** consulta de información climática e histórica.
- **Personal y estudiantes del campus:** visualización de las condiciones climáticas locales.

## Objetivo
Implementar una estación meteorológica IoT automatizada basada en hardware y un ESP32 para recopilar datos climáticos locales, almacenarlos en SQL Server, generar análisis y alertas mediante reglas definidas en el proyecto y presentar los resultados mediante una interfaz amigable.

## Descripción general
UNICLIMA METRICS contempla una estación meteorológica de bajo costo construida alrededor de un ESP32.

- **BMP280:** temperatura y presión barométrica.
- **DHT11:** humedad relativa.
- **FC-37:** detección de precipitación.
- **Sensor UV:** medición de radiación ultravioleta.
- Comunicación mediante **Wi-Fi y HTTP** dentro de la red de la universidad.
- Persistencia de datos en **SQL Server**.

El sistema contempla visualización dinámica mediante indicadores tipo semáforo, alertas de UV, cálculo aproximado del tiempo seguro de exposición solar, detección de posibles condiciones de tormenta o frente frío mediante variaciones de presión, cálculo de un índice acumulativo de sequía, administración de estaciones, consulta histórica y reportes en PDF y Excel.

## Integrantes
- **Camila Raquel Choque Peñafiel** — Grupo: UNNICLIMA METRICS — Rol: pendiente de definir.
- **José Carlos Trujillo Soliz** — Grupo: Paralelo 3 — Rol: pendiente de definir.

> Los roles se mantienen como pendientes porque el informe proporcionado no especifica las responsabilidades individuales.

## Estado actual
**Hito 2 — Definición y alcance.**

Actualmente se han establecido la problemática, objetivos, requisitos funcionales y no funcionales, alcance, limitaciones, historias de usuario, metodología Scrum, selección inicial de sensores y hardware, arquitectura general de comunicación, uso de SQL Server y los hitos de desarrollo.

### Próximos hitos
- **Hito 3:** primer prototipo funcional, base de datos física, conexión del ESP32 con sensores y primera visualización.
- **Hito 4:** sistema al 90%, algoritmos de sequía y detección barométrica, panel administrativo y UML consolidado.
- **Hito 5:** sistema final al 100%, pruebas de integración, correcciones, documentación final y defensa.

## Organización del repositorio

```text
PEP2-2026-PROYECTO/
├── README.md
├── docs/
├── src/
├── database/
├── tests/
├── resources/
├── EQUIPO/
└── .github/
```

## Metodología
El proyecto utiliza **Scrum**, contemplando refinamiento, planificación de Sprint, construcción, revisión y retrospectiva.

## Alcance
El proyecto está orientado al monitoreo climático dentro de las áreas del campus de UNIFRANZ y contempla un prototipo universitario de bajo costo.

No se contempla en la fase actual:
- Modelos de predicción mediante redes neuronales o aprendizaje automático complejo.
- Una carcasa meteorológica industrial.
- Aplicaciones nativas para Android o iOS.
- Pronósticos fuera de las áreas del campus de UNIFRANZ.

> **Nota:** el informe menciona tanto una aplicación web como Windows Forms/C#. Esta definición tecnológica deberá aclararse antes de implementar la estructura definitiva de la aplicación.