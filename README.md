```markdown
# 🧪 TechMarket - Suite de Pruebas Automatizadas

## 🎯 Objetivo del Proyecto

Validar el correcto funcionamiento, seguridad y robustez de la API REST de **TechMarket** mediante pruebas manuales, automatizadas y generación de reportes. Se aplicaron buenas prácticas de diseño, mitigación de amenazas y herramientas especializadas para asegurar la calidad del sistema.


## 🔍 ¿Qué es una API REST?

Una API REST es un estilo arquitectónico basado en HTTP que permite la comunicación entre sistemas mediante recursos identificados por URLs. Utiliza métodos estándar (`GET`, `POST`, `PUT`, `DELETE`) y formatos como JSON para intercambiar datos.

### 📌 Recursos expuestos por la API de TechMarket

- **Gestión de productos**: `/api/v1/products`
- **Registro y autenticación de usuarios**: `/api/v1/auth`


## ⚙️ Componentes principales de una API REST

| Componente       | Ejemplo en TechMarket                                             |
|------------------|-------------------------------------------------------------------|
| Recurso          | `/products`, `/auth`                                              |
| Método HTTP      | `GET`, `POST`, `PUT`, `DELETE`                                    |
| Endpoint         | `GET /api/v1/products`, `POST /api/v1/auth/login`                 |
| Body (JSON)      | `{ "name": "Laptop", "price": 999.99 }`                           |
| Headers          | `Content-Type: application/json`, `Authorization: Bearer <token>` |
| Códigos HTTP     | `200 OK`, `201 Created`, `404 Not Found`, `401 Unauthorized`      |



## 🛠️ Herramientas Utilizadas

| Herramienta     | Propósito                                                  |
|-----------------|------------------------------------------------------------|
| **Postman**     | Pruebas manuales, exploración de endpoints, colección base |
| **Newman**      | Ejecución automatizada de colecciones Postman vía CLI      |
| **Rest-Assured**| Pruebas automatizadas en Java, validación de respuestas    |



## ✅ Buenas Prácticas Aplicadas

- **Versionado de API**: `/api/v1/...`
- **Uso de DTOs**: `ProductDTO` para entrada/salida
- **Validación**: Anotaciones `@Valid` en controladores
- **Excepciones personalizadas**: `ResourceNotFoundException`
- **Códigos de estado correctos**: `201 Created`, `204 No Content`
- **Seguridad**: Autenticación con JWT, encriptación con `PasswordEncoder`
- **Registro RESTful**: Uso de `Location` header en respuestas `POST`



## 🔐 Amenazas de Seguridad y Mitigaciones

| Amenaza                  | Mitigación Implementada                                     |
|--------------------------|-------------------------------------------------------------|
| Acceso no autorizado     | JWT en endpoints protegidos                                 |
| Credenciales débiles     | Validación con `@Valid`, encriptación con `PasswordEncoder` |
| Exposición de datos      | Uso de `ProductDTO`, no se expone `password`                |
| Usuarios duplicados      | Validación con `existsByEmail()`                            |
| Tokens reutilizables     | Control con `tokenVersion` en `UserAccount`                 |
| Auditoría                | Logs y capturas agregadas para trazabilidad                 |



## 📁 Estructura del Proyecto

```bash
TechMarket-Tests/
├── postman/
│   ├── TechMarket.postman_collection.json
│   └── environment.json
├── newman/
│   └── report.html
├── rest-assured/
│   ├── src/test/java/com/techmarket/api/
│   └── pom.xml
├── README.md
```



## 📊 Resultados y Evidencias

- Colección Postman con pruebas funcionales y de seguridad
- Reporte HTML generado por Newman
- Pruebas automatizadas con Rest-Assured
- Logs y capturas disponibles para auditoría técnica


## 🗣️ Defensa Técnica

Este proyecto demuestra la capacidad de aplicar pruebas manuales y automatizadas sobre una API REST moderna, con enfoque en seguridad, buenas prácticas y trazabilidad. Las decisiones técnicas están justificadas en base a estándares REST, mitigación de riesgos y uso eficiente de herramientas.


## 📌 Autor

Mauricio Vera 
Desarrollador Full Stack | Técnico en Informática y Telecomunicaciones  
Especialista en QA y automatización

```
