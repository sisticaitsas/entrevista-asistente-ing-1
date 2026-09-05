# Prueba Técnica – Asistente de Ingeniería

## Parte 1. Reto de desarrollo

### 1. Contexto

Una empresa necesita mejorar la forma en que sus colaboradores reportan y hacen seguimiento a **incidencias asociadas a equipos, espacios o recursos internos**.

Cada activo o ubicación podrá tener asociado un **código QR**. Al escanearlo, el usuario deberá acceder a una aplicación web desde la cual pueda registrar una incidencia.

El equipo administrativo deberá contar con un panel que permita consultar, clasificar, gestionar y analizar los reportes recibidos.

El objetivo de la prueba es evaluar capacidades de **desarrollo Full Stack, arquitectura, APIs, bases de datos, seguridad, UX/UI, pruebas, contenedores y organización del código**.

---

# 2. Flujo de usuario

Al escanear un código QR, el usuario deberá acceder a una página de reporte.

El formulario deberá solicitar como mínimo:

- Nombre.
- Apellido.
- Correo corporativo.
- Teléfono.
- Tipo de incidencia.
- Descripción de la incidencia.

El código QR deberá permitir identificar automáticamente algún elemento dentro del sistema, por ejemplo:

- Equipo.
- Ubicación.
- Recurso.
- Área.

Ejemplo:

`QR → Equipo portátil #A023 → Formulario de reporte`

### Requisitos

El sistema deberá:

- Validar correctamente los campos.
- Validar tanto desde frontend como desde backend.
- Registrar la información en una base de datos.
- Relacionar el reporte con el recurso identificado mediante el QR.
- Generar una confirmación cuando el reporte se registre correctamente.
- Mostrar mensajes adecuados cuando ocurra un error.
- Priorizar el funcionamiento desde dispositivos móviles.

---

# 3. Panel administrativo

El sistema deberá incluir un panel administrativo protegido mediante autenticación.

El administrador deberá poder iniciar sesión y acceder únicamente a las funcionalidades autorizadas.

## Gestión de incidencias

Desde el panel deberá ser posible:

- Visualizar los reportes registrados.
- Consultar el detalle de cada reporte.
- Identificar el activo o recurso relacionado.
- Consultar información del usuario que realizó el reporte.
- Modificar el estado de una incidencia.
- Clasificar las incidencias.

Como mínimo deberá existir una clasificación relacionada con prioridad:

- Baja.
- Media.
- Alta.

El candidato puede agregar otras clasificaciones si considera que aportan valor.

---

# 4. Gestión mediante Kanban

Las incidencias deberán poder gestionarse utilizando un tablero visual tipo **Kanban**.

Como mínimo deberá incluir las siguientes etapas:

**Reportado → En revisión → En proceso → Resuelto**

El sistema deberá permitir cambiar una incidencia de estado.

Se valorará positivamente que el cambio pueda realizarse mediante **Drag & Drop**, aunque no será obligatorio.

Cada tarjeta deberá mostrar información suficiente para identificar rápidamente la incidencia.

Por ejemplo:

- Código.
- Tipo.
- Prioridad.
- Fecha.
- Recurso asociado.

---

# 5. Dashboard y métricas

El panel administrativo deberá presentar métricas relacionadas con la operación.

Como mínimo deberá mostrar:

- Total de incidencias.
- Incidencias abiertas.
- Incidencias resueltas.
- Incidencias agrupadas por prioridad.
- Reportes registrados por fecha.
- Porcentaje de incidencias resueltas.

El candidato decidirá cómo representar la información.

Podrá utilizar:

- Tarjetas.
- Tablas.
- Barras.
- Gráficas.
- Indicadores.

Se evaluará principalmente que la información sea **comprensible y útil**, no la complejidad de las visualizaciones.

---

# 6. Requisitos técnicos

La solución deberá cumplir como mínimo con:

- Desarrollo **Frontend + Backend**.
- Framework de libre elección.
- API para comunicación entre frontend y backend.
- Persistencia en una **base de datos**.
- Autenticación mediante **JWT (JSON Web Token)**.
- Protección de las rutas administrativas.
- Validación de información en frontend y backend.
- Manejo adecuado de errores.
- Uso de variables de entorno para información de configuración.
- Proyecto **dockerizado**.
- Pruebas automatizadas.
- Código estructurado y organizado.
- Control de versiones utilizando **Git**.
- Repositorio donde pueda revisarse el historial del proyecto.

No se evaluará negativamente la elección de una tecnología particular siempre que el candidato pueda justificarla.

---

# 7. UX/UI

La experiencia de usuario constituye una parte importante de la evaluación.

Se espera como mínimo:

- Diseño responsive.
- Correcta visualización desde dispositivos móviles.
- Navegación intuitiva.
- Formularios claros.
- Buena jerarquía visual.
- Estados de carga.
- Estados de error.
- Estados de éxito.
- Feedback visual después de las acciones.
- Panel administrativo fácil de interpretar.
- Consistencia visual.

No se exige ninguna librería específica de componentes.

---

# 8. Entregables

El candidato deberá entregar:

1. **URL del repositorio** que contenga el código fuente.

2. Archivo `README.md` con:
   - Descripción del proyecto.
   - Arquitectura general utilizada.
   - Tecnologías seleccionadas.
   - Instrucciones de instalación.
   - Instrucciones de ejecución.
   - Variables de entorno necesarias.
   - Instrucciones para ejecutar las pruebas.
   - Instrucciones para levantar el proyecto con Docker.

3. Configuración necesaria de **Docker**.

4. Código QR o URL que permita probar el flujo de creación de incidencias.

5. Credenciales de prueba para acceder al panel administrativo.

6. Breve explicación de las principales decisiones técnicas tomadas durante el desarrollo.

---

# 9. Criterios de evaluación

| Criterio | Peso |
|---|---:|
| Funcionamiento general | 25% |
| Calidad y organización del código | 20% |
| UX/UI | 15% |
| Backend, API y base de datos | 15% |
| Seguridad y autenticación JWT | 10% |
| Pruebas automatizadas | 10% |
| Docker, documentación y facilidad de ejecución | 5% |
| **Total** | **100%** |

---

# 10. Aspectos adicionales

Se considerarán positivamente, pero **no son obligatorios**:

- Documentación de la API.
- Swagger / OpenAPI.
- Migraciones de base de datos.
- Filtros.
- Búsqueda.
- Paginación.
- Drag & Drop en Kanban.
- Gráficas.
- Logs.
- Buen manejo de excepciones.
- Buenas prácticas de seguridad.
- Uso correcto de variables de entorno.
- Despliegue de una versión funcional.
- Arquitectura preparada para crecimiento.
- Pruebas de integración además de pruebas unitarias.

Estos elementos no deberán utilizarse para compensar funcionalidades obligatorias que no hayan sido implementadas.

---

# Parte 2. Evaluación técnica de ciberseguridad

Responder de manera breve y técnica las siguientes preguntas.

## 1. Autenticación y JWT

Una aplicación utiliza JWT para proteger el panel administrativo.

Explique:

- ¿Qué información debería y no debería almacenarse dentro de un JWT?
- ¿Dónde almacenaría el token en una aplicación web y qué riesgos existen?
- ¿Cómo manejaría la expiración del token?
- ¿Qué diferencia existe entre un `access token` y un `refresh token`?

---

## 2. Contraseñas

El sistema requiere almacenar las credenciales de los administradores.

Explique:

- ¿Cómo almacenaría una contraseña correctamente?
- ¿Por qué no debería almacenarse utilizando cifrado reversible?
- Mencione al menos un algoritmo apropiado para almacenar contraseñas.

---

## 3. SQL Injection

Considere una API que recibe un parámetro ingresado por un usuario y lo utiliza para consultar una base de datos.

Explique:

- ¿Qué es una inyección SQL?
- ¿Cómo podría producirse?
- ¿Qué mecanismos utilizaría para prevenirla?

---

## 4. XSS

Explique qué es un ataque **Cross-Site Scripting (XSS)** y mencione medidas para reducir el riesgo dentro de una aplicación web.

---

## 5. Control de acceso

Suponga que existe el siguiente endpoint:

`GET /api/incidents/125`

El usuario autenticado modifica manualmente la URL y consulta:

`GET /api/incidents/126`

La incidencia `126` pertenece a otro usuario al que no debería tener acceso.

Responda:

- ¿Qué vulnerabilidad podría existir?
- ¿Dónde debería realizarse la validación?
- ¿Cómo la solucionaría?

---

## 6. Variables de entorno

Explique por qué elementos como los siguientes no deberían almacenarse directamente dentro del código fuente:

- Contraseñas.
- Secretos JWT.
- API Keys.
- Credenciales de bases de datos.

Indique una forma adecuada de administrarlos.

---

## 7. Docker

Suponga que encuentra lo siguiente dentro de un `Dockerfile`:

`ENV DATABASE_PASSWORD=MiPasswordProduccion123`

Explique:

- ¿Cuál es el problema?
- ¿Qué riesgo representa?
- ¿Cómo debería manejarse correctamente?

---

## 8. Caso práctico

Después de desplegar la aplicación, comienza a recibir cientos de solicitudes automáticas al formulario público generado desde el QR.

Indique qué controles implementaría para reducir:

- Automatización maliciosa.
- Spam.
- Abuso de la API.
- Saturación del servicio.

Justifique brevemente las decisiones.

---

# Consideraciones finales

La tecnología queda a elección del candidato.

No buscamos únicamente verificar que una aplicación funcione.

Se evaluará también la capacidad para:

**Analizar → Diseñar → Implementar → Validar → Proteger → Documentar**

Se tendrá en cuenta especialmente la capacidad del candidato para justificar sus decisiones técnicas y construir una solución comprensible, mantenible y ejecutable.
