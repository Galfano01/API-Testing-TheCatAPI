# API Testing Project – The Cat API

## Descripción

Este proyecto contiene el diseño y ejecución de casos de prueba realizados sobre The Cat API, con el objetivo de validar el correcto funcionamiento de los endpoints, aplicar
pruebas positivas y negativas, y documentar defectos encontrados.

El enfoque del proyecto está basado en buenas prácticas de QA, incluyendo:

- Diseño estructurado de casos de prueba
- Ejecución documentada
- Gestión de defectos
- Evidencia de pruebas
- Métricas de ejecución

---

## Alcance de Pruebas

Se validaron los siguientes módulos:

- Breeds
- Images
- Votes

Endpoints probados:

- GET /v1/breeds
- GET /v1/images/search
- POST /v1/votes
- GET /v1/votes
- DELETE /v1/votes/{id}

---

##  Resumen de Ejecución

| Métrica | Resultado |
|----------|------------|
| Total Casos Ejecutados | 10 |
| Casos Exitosos | 8 |
| Casos Fallidos | 2 |
| Porcentaje de Éxito | 80% |

Ambiente de pruebas: QA  
Tipo de pruebas: Funcionales (positivas y negativas)

---

##  Defectos Detectados

### BUG-001 – Falta de validación de rango en campo `value`

El endpoint POST /v1/votes permite registrar valores fuera del rango esperado (ejemplo: value = 23), retornando código 201 en lugar de 400.

Impacto: Se incumple la regla de negocio esperada.

---

### BUG-002 – Falta de validación de tipo de dato en campo `value`

El endpoint POST /v1/votes permite registrar valores tipo string (ejemplo: "hola"), retornando código 201 en lugar de 400.

Impacto: No existe validación de tipo de dato, lo que puede generar inconsistencias en la base de datos.

---
## Objetivo Profesional

Este proyecto fue desarrollado como práctica de aseguramiento de calidad para fortalecer habilidades en:

- Diseño de Casos de Prueba
- Validaciones API
- Pruebas Negativas
- Detección y documentación de defectos
- Reporte de métricas de ejecución

---

## Autor

Jeysson Monterrosa  
QA Manual Tester
