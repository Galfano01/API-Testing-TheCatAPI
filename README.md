# API Testing Project – The Cat API

## Descripción
Proyecto de pruebas funcionales realizadas sobre la API pública The Cat API, con el objetivo de validar el comportamiento de los endpoints principales mediante pruebas positivas y negativas.

---

## Objetivo del Proyecto
- Diseñar casos de prueba funcionales.
- Ejecutar pruebas sobre endpoints REST.
- Validar códigos de respuesta HTTP.
- Detectar defectos en validación de datos.
- Documentar resultados y evidencias.

---

## Endpoints Evaluados

| Endpoint |  Método  | Descripción |
|----------|----------|------------|
| /v1/breeds | GET    | Lista de razas |
| /v1/images/search | GET | Búsqueda de imágenes |
| /v1/votes | POST | Crear voto |
| /v1/votes/{id} | DELETE | Eliminar voto |

---

##  Casos de Prueba

- Total casos diseñados: 10
- Casos exitosos: 8
- Casos fallidos: 2

---

## Defectos Detectados

1. El endpoint POST /v1/votes permite registrar valores fuera del rango esperado.
2. El endpoint POST /v1/votes permite enviar valores tipo string sin validación.

Impacto: Posible inconsistencia en la integridad de datos.

---

## Herramientas Utilizadas

- Postman
- Excel
- GitHub

---

## 📂 Evidencias

Las evidencias de ejecución se encuentran en el documento de ejecucion de pruebas.

---

## 👨‍💻 Autor

Proyecto realizado como práctica de QA Manual para fortalecimiento de habilidades en pruebas de API.
