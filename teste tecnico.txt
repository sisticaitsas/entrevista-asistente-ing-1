# Prueba Técnica – Asistente ingenieria:

## 1. Objetivo

Desarrollar una **plataforma web Full Stack (Frontend + Backend)** que permita captar los datos de un cliente a partir del acceso mediante un **código QR**.

La prueba busca evaluar conocimientos de desarrollo, arquitectura básica, manejo de bases de datos, autenticación, experiencia de usuario, pruebas y despliegue mediante contenedores.

---

## 2. Funcionalidades requeridas

### A. Módulo de Usuario

Al escanear el código QR, el usuario deberá acceder a una página con un formulario de registro.

El formulario deberá solicitar como mínimo:

* Nombre
* Apellido
* Correo corporativo
* Teléfono

### Requisitos

* Validar correctamente los campos.
* Guardar la información en una base de datos.
* Mostrar una confirmación cuando el registro se complete exitosamente.
* Priorizar una experiencia sencilla, rápida y visualmente clara, especialmente desde dispositivos móviles.

---

### B. Módulo Administrativo

Crear un panel de administración protegido mediante autenticación.

El administrador deberá poder:

#### Gestión de registros

* Visualizar los usuarios registrados.
* Consultar la información de cada registro.
* Clasificar cada contacto como:

  * **Prospecto**
  * **Cliente**

#### Tablero Kanban

Crear un tablero tipo **Kanban** que permita gestionar visualmente los registros.

Como mínimo, deberá permitir mover los contactos entre diferentes estados o etapas.

Ejemplo:

**Nuevo → Prospecto → Cliente**

#### Métricas

El panel deberá presentar algunas métricas básicas, por ejemplo:

* Total de registros.
* Número de prospectos.
* Número de clientes.
* Registros realizados por fecha.
* Conversión de prospectos a clientes.

La forma de visualizar estas métricas queda a criterio del desarrollador.

---

## 3. Requisitos técnicos

El proyecto deberá cumplir con los siguientes requisitos:

* Desarrollo **Frontend + Backend**.
* Utilizar un framework de elección libre.
* Persistencia de información en una **base de datos**.
* Implementar autenticación mediante **JWT (JSON Web Token)**.
* Proteger las rutas administrativas.
* Implementar validaciones tanto en frontend como en backend.
* El proyecto deberá estar **dockerizado**.
* Incluir pruebas automatizadas.
* Mantener una estructura de código clara y organizada.
* Utilizar control de versiones con **Git**.
* Publicar el proyecto en un repositorio.

---

## 4. UX/UI

La experiencia de usuario tendrá un peso importante dentro de la evaluación.

Se espera:

* Diseño responsive.
* Buena visualización en dispositivos móviles.
* Navegación intuitiva.
* Formularios claros.
* Jerarquía visual adecuada.
* Estados de carga, éxito y error.
* Panel administrativo fácil de entender.
* Consistencia visual entre las diferentes secciones.

No se exige utilizar una librería de componentes específica.

---

## 5. Entregables

El candidato deberá entregar:

1. **URL del repositorio** con el código fuente.
2. Archivo `README.md` con:

   * Descripción del proyecto.
   * Tecnologías utilizadas.
   * Instrucciones de instalación.
   * Instrucciones para ejecutar el proyecto.
   * Instrucciones para ejecutar las pruebas.
   * Variables de entorno necesarias.
3. Archivo o configuración de **Docker** para levantar el proyecto.
4. Código QR o URL que permita probar el flujo de registro.
5. Credenciales de prueba para ingresar al panel administrativo.

---

## 6. Criterios de evaluación

| Criterio                                       | Peso |
| ---------------------------------------------- | ---: |
| Funcionamiento general                         |  25% |
| Calidad y organización del código              |  20% |
| UX/UI                                          |  15% |
| Backend, API y base de datos                   |  15% |
| Seguridad y autenticación JWT                  |  10% |
| Pruebas                                        |  10% |
| Docker, documentación y facilidad de ejecución |   5% |

---

## 7. Aspectos adicionales

Se valorarán positivamente, aunque **no son obligatorios**:

* Buen manejo de errores.
* Documentación de la API.
* Uso correcto de variables de entorno.
* Migraciones de base de datos.
* Filtros o búsqueda de registros.
* Paginación.
* Drag & Drop en el tablero Kanban.
* Gráficas para las métricas.
* Buenas prácticas de seguridad.
* Despliegue de una versión funcional en línea.

---

## 8. Consideraciones

La tecnología utilizada queda a elección del candidato.

No buscamos únicamente que la aplicación funcione. Se evaluará también **cómo está pensada, estructurada y construida**.

Se priorizarán:

**Claridad → Funcionalidad → UX/UI → Calidad del código → Buenas prácticas.**


*****2 parte:*******

Peguntas tecnicas: ciberseguridad
