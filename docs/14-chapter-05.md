# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

En esta sección se describen las decisiones, convenciones y principios adoptados por el equipo de **RQLS** para garantizar la coherencia, trazabilidad y control de versiones durante el ciclo de vida del desarrollo de la solución **Buildline**. Se establecen los lineamientos para la configuración del entorno de desarrollo, gestión del código fuente, convenciones de estilo y configuración de despliegue orientada a la nube.

### 5.1.1. Software Development Environment Configuration

Se especifican los productos de software utilizados durante el ciclo de vida del proyecto, organizados por disciplinas técnicas para asegurar la estandarización del entorno entre los desarrolladores de Buildline.

#### Project Management
* **Jira:** Utilizada para la gestión de la metodología Scrum, administración del Product Backlog, planificación de Sprints y seguimiento de User Stories para el control logístico de obra.
    * **Ruta:** [https://www.atlassian.com/software/jira](https://www.atlassian.com/software/jira)

#### Requirements Management
* **Trello:** Empleado para la organización visual del flujo de trabajo diario y la priorización rápida de tareas durante el desarrollo de los módulos de requisición.
    * **Ruta:** [https://trello.com](https://trello.com)

#### Product UX/UI Design
1.  **Miro:** Pizarra colaborativa fundamental para el Design-Level Event Storming de Buildline, permitiendo identificar los eventos de dominio entre obra y oficina.
2.  **Figma:** Herramienta principal para el diseño de la interfaz móvil (Field App) y la plataforma web de gestión, incluyendo el diseño del sistema de diseño (Design System).
3.  **LucidChart:** Utilizado para el modelado de la arquitectura de software mediante diagramas C4 y diagramas de base de datos relacional.

#### Software Development
1.  **GitHub:** Hosting de repositorios bajo la organización RQLS. Implementación de GitFlow para separar las funcionalidades de inventario, compras y reportes.
2.  **WebStorm:** IDE especializado para el desarrollo del Frontend de Buildline, optimizando la codificación con Vue.js y la gestión de estilos.
3.  **JetBrains Rider:** IDE principal para el desarrollo del Backend robusto basado en .NET/C#, facilitando la integración con servicios de base de datos y lógica de negocio.
4.  **Vue.js Framework:** Framework progresivo de JavaScript elegido para construir la SPA de Buildline por su ligereza y velocidad de carga en condiciones de baja conectividad en obra.
5.  **.NET 8 / C#:** Tecnología de backend para garantizar la escalabilidad, seguridad transaccional en las Órdenes de Compra y alto rendimiento.

#### Software Testing
* **Lenguaje Gherkin:** Utilizado para definir los criterios de aceptación en formato Given-When-Then, asegurando que las validaciones de "Way Match" y presupuestos funcionen correctamente.

#### Software Documentation
* **Swagger / OpenAPI:** Generación de documentación interactiva para que el equipo de Frontend pueda consumir los servicios de requisiciones y proveedores de forma eficiente.

---

### 5.1.2. Source Code Management

Se establecen los repositorios oficiales de la solución Buildline para garantizar la integridad del código fuente.

#### Repositorios del Proyecto
<table>
  <thead>
    <tr>
      <th>Producto</th>
      <th>URL del Repositorio</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Organización ClosedSource-11848</td>
      <td><a href="https://github.com/RQLS26">https://github.com/RQLS26</a></td>
    </tr>
    <tr>
      <td>Landing Page</td>
      <td><a href="https://github.com/RQLS26-LandingPage">https://github.com/RQLS26-LandingPage</a></td>
    </tr>
    <tr>
      <td>Frontend Web Application</td>
      <td><a href="https://github.com/RQLS26-Frontend">https://github.com/RQLS26--Frontend</a></td>
    </tr>
    <tr>
      <td>Backend Web Services</td>
      <td><a href="https://github.com/RQLS26-Backend">https://github.com/RQLS26-Backend</a></td>
    </tr>
  </tbody>
</table>

#### GitFlow Workflow
* **main:** Código estable y auditado desplegado en producción.
* **develop:** Rama base para integración de nuevas características.
* **feature/&lt;módulo&gt;:** Ej: `feature/procurement-comparison-sheet`.
* **hotfix/&lt;issue&gt;:** Parches rápidos para errores críticos en el cálculo de APU.

<h4>Conventional Commits</h4>
<pre><code>feat(tracking): implement IoT telemetry ingestion endpoint
fix(compliance): resolve stock update discrepancy on partial receipt
docs(readme): update swagger definitions for supplier endpoints
build(deps): migrate to .NET 8.0 SDK
</code></pre>


### 5.1.3. Source Code Style Guide & Conventions

En esta sección se establecen las convenciones de estilo y nomenclatura adoptadas para los lenguajes utilizados en el proyecto Buildline: HTML, CSS, JavaScript, TypeScript (Vue.js), C# (.NET 8) y Gherkin. Se aplica nomenclatura en inglés para todos los elementos del código, siguiendo el Ubiquitous Language definido para el dominio logístico de la construcción.

#### Referencias de Guías de Estilo Adoptadas

| Lenguaje/Tecnología | Guía de Estilo |
| :--- | :--- |
| HTML/CSS | [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html) |
| JavaScript | [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html) |
| TypeScript / Vue.js | [Vue.js Priority A Guide](https://vuejs.org/style-guide/rules-essential.html) |
| C# / .NET | [Microsoft C# Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions) |
| Java | [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html) 
| Gherkin | [Gherkin Reference](https://cucumber.io/docs/gherkin/reference/) |

Se utiliza nomenclatura en inglés relacionada con las entidades del dominio logístico (ej. Requisition, Quote, Inventory, Provider).

| Elemento | Convención | Ejemplo |
| :--- | :--- | :--- |
| Clases C# | PascalCase | `PurchaseOrderService`, `BudgetController` |
| Interfaces C# | PascalCase (prefijo I) | `IRequisitionRepository` |
| Métodos C# | PascalCase | `CalculateOvercost()`, `ApproveOrder()` |
| Variables / Métodos TS | camelCase | `materialId`, `fetchQuotes()` |
| Constantes | SCREAMING_SNAKE_CASE | `MIN_STOCK_LEVEL`, `MAX_FILE_SIZE` |
| Componentes Vue | kebab-case (archivos) | `quote-comparison-table.vue` |

#### Sangría y Formato
* Se aplica una indentación de dos espacios para archivos web (HTML, CSS, TS) y de cuatro espacios para C# (estándar de Rider/Visual Studio).
* Las llaves de apertura en C# se colocan en una nueva línea (Estilo Allman), mientras que en TS/JS van en la misma línea (Estilo K&R).

---
### 5.1.4. Software Deployment Configuration

Se especifica la configuración de despliegue para los entornos de Buildline, garantizando alta disponibilidad para ingenieros en obra.

#### Landing Page - GitHub Pages
Despliegue automático del contenido estático mediante GitHub Actions tras cada merge a la rama `main`.
* **URL:** [https://github.com/RQLS26-LandingPage](https://github.com/RQLS26-LandingPage)

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th colspan="2" style="text-align: center;">Sprint Planning Sprint 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Planning Background</strong></td>
    </tr>
    <tr>
      <td>Date</td>
      <td>05/04/2026</td>
    </tr>
    <tr>
      <td>Time</td>
      <td>10:00 p.m.</td>
    </tr>
    <tr>
      <td>Location</td>
      <td>Discord / Whatsapp</td>
    </tr>
    <tr>
      <td>Prepared By</td>
      <td>Castillo Yataco, Mauricio Sebastián</td>
    </tr>
    <tr>
      <td>Attendees</td>
      <td>
        Castillo Yataco, Mauricio Sebastián<br>
        Morales Venegas, David Joel<br>
        Paucar Zenteno, Jesús Fernando<br>
        Viza Quispe, Marlon Packard<br>
        Cáceres Pizarro, Albino Florencio
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Goal & User Stories</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint 1 Goal (Outcome–Impact–Customer–Confirmation):</strong><br><br>
<em>Our focus is on delivering the first marketing Landing Page of Buildline that clearly communicates the value proposition regarding logistics traceability and APU budget control.</em><br><br>
<em>We believe it delivers a clear, professional first impression for Project Managers and General Managers of construction MYPES, helping them understand our SaaS offering.</em><br><br>
<em>This will be confirmed when users can navigate through all core sections (Hero, Features, Benefits, Plans, About Us) and can seamlessy contact the sales team.</em>
      </td>
    </tr>
    <tr>
      <td>Sprint 1 Velocity</td>
      <td>14 Story Points</td>
    </tr>
  </tbody>
</table>
<p>
  <strong>Repositorio:</strong> <a href="https://github.com/RQLS26-LandingPage">https://github.com/RQLS26-LandingPage</a>
</p>
#### 5.2.1.2. Aspect Leaders and Collaborators

<p>
Esta matriz <strong>LACX</strong> identifica los aspectos principales del sprint y asigna responsabilidades (Líder/Colaborador) para organizar al equipo de RQLS.
</p>

<table border="1" cellpadding="4" cellspacing="0" align="center">
  <thead>
    <tr>
      <th>Team Member</th>
      <th>Aspect: UI/UX & Styling</th>
      <th>Aspect: HTML Structuring & Deployment</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Castillo Yataco, Mauricio Sebastián</td><td>L</td><td>C</td></tr>
    <tr><td>Morales Venegas, David Joel</td><td>C</td><td>L</td></tr>
    <tr><td>Paucar Zenteno, Jesús Fernando</td><td>C</td><td>C</td></tr>
    <tr><td>Viza Quispe, Marlon Packard</td><td>C</td><td>C</td></tr>
    <tr><td>Cáceres Pizarro, Albino Florencio</td><td>C</td><td>C</td></tr>
  </tbody>
</table>

### 5.2.1.3. Sprint Backlog 1  

El Sprint Backlog agrupa las tareas iniciales correspondientes a la presencia digital del proyecto Buildline.

<div align="center">
  <img src="./assets/chapter-05/jira1.png" alt="Sprint 1 Board Screenshot" width="100%">
  <p><em>Figura: Tablero del Sprint 1 en Jira Software (Proyecto Buildline)</em></p>
</div>

| User Story Id | Title | Task Id | Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **US00** | Landing Page Base | T001 | Implementación de Hero y Features | Desarrollo de la sección principal y propuesta de valor en HTML/CSS/Vue.js. | 4h | Morales Venegas, David Joel | Done |
| **US00** | Landing Page Info | T002 | Maquetación de Beneficios | Implementación de la sección informativa detallando el control de APU y la trazabilidad logística. | 3h | Castillo Yataco, Mauricio Sebastian | Done |
| **Cap I - II** | Discovery & Discovery | T003 | Needfinding y Strategic Domain | Análisis de entrevistas con gerentes de obra, Lean UX Canvas y definición del Ubiquitous Language. | 6h | Viza Quispe, Marlon | Done |
| **Cap II - III** | Requirements Eng. | T004 | Context Mapping y Product Backlog | Definición del Mapa de Contexto (DDD), Impact Mapping y redacción de User Stories (Gherkin). | 5h | Paucar Zenteno, Jesus Fernando | Done |
| **Cap IV** | Software Design | T005 | Event Storming y C4 Model | Sesión de Design-Level Event Storming y elaboración de diagramas de Contexto y Contenedores en Structurizr. | 7h | Cáceres Pizarro, Albino Florencio | Done |

#### 5.2.1.4. Development Evidence for Sprint Review

<p>
  Resumen de los commits más relevantes en el repositorio de la Landing Page de Buildline.
</p>

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>Branch</th>
      <th>Commit Id</th>
      <th>Commit Message</th>
      <th>Committed on</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>main</td>
      <td><code>42086bfb18d1f9d3eb360d40cbebbd3298126335</code></td>
      <td>docs: finalize needfinding analysis and lean UX canvas (Cap I)</td>
      <td>10-04-2026</td>
    </tr>
    <tr>
      <td>feature/landing</td>
      <td><code>8b5f6d2</code></td>
      <td>feat(ui): implement landing page hero and feature sections</td>
      <td>22-04-2026</td>
    </tr>
    <tr>
      <td>feature/ddd-design</td>
      <td><code>3c9a8b1</code></td>
      <td>docs(ddd): define strategic context map and ubiquitous language</td>
      <td>18-04-2026</td>
    </tr>
    <tr>
      <td>feature/architecture</td>
      <td><code>7903d32</code></td>
      <td>docs(c4): complete system context and container diagrams in DSL</td>
      <td>19-04-2026</td>
    </tr>
    <tr>
      <td>main</td>
      <td><code>0a8cdee</code></td>
      <td>docs: update product backlog and impact mapping (Cap III)</td>
      <td>13-04-2026</td>
    </tr>
  </tbody>
</table>

#### 5.2.1.5. Execution Evidence for Sprint Review

<p>
  Se completó la implementación y el diseño de la Landing Page.
</p>

#### 5.2.1.6. Services Documentation Evidence
<p>
  Dado que el Sprint 1 abarca únicamente contenido estático (Landing Page de marketing), la implementación y consumo de la API en .NET para la gestión de requisiciones y órdenes de compra se abordará en los sprints posteriores orientados al Backend Web Services.
</p>

#### 5.2.1.7. Software Deployment Evidence
<p>
  <strong>URL de Producción:</strong> <a href="https://github.com/RQLS26-LandingPage">https://github.com/RQLS26-LandingPage/</a>
</p>

#### 5.2.1.8. Team Collaboration Insights during Sprint

<p>
  Durante este primer sprint, el esfuerzo principal del equipo de RQLS se centró en la estructuración del proyecto, el diseño de UX/UI, la arquitectura de software y la elaboración de los requerimientos técnicos (Capítulos I al IV). Por lo tanto, las evidencias de colaboración de GitHub presentadas a continuación corresponden al repositorio del <strong>Project Report</strong>, sentando las bases documentales y de diseño para la posterior codificación de la plataforma Buildline.
</p>

<p>
  En primer lugar, el <strong>Historial de Commits</strong> del repositorio demuestra que el trabajo no fue centralizado, sino altamente colaborativo. A lo largo del sprint, se observa un flujo constante de aportes realizados en diferentes días por distintos miembros del equipo (reflejados a través de sus usuarios de GitHub). Cada integrante se encargó de actualizar y mejorar secciones específicas, como el análisis de entrevistas a los Gerentes y Residentes, el Event Storming o los diagramas de arquitectura C4, evidenciando un desarrollo incremental y distribuido.
</p>

<div align="center">
  <img src="../docs/assets/chapter-05/commit-history-sprint1.png" alt="Commit History Evidence" width="90%">
  <p><em>Figura: Historial de commits demostrando la participación activa de los miembros del equipo RQLS.</em></p>
</div>

<p>
  En segundo lugar, el gráfico de <strong>Visitors (Traffic)</strong> proporcionado por los Insights de GitHub demuestra que el repositorio documental mantuvo una actividad de consulta constante. El flujo de "Views" y "Unique visitors" a lo largo de las semanas del sprint confirma que los integrantes del equipo ingresaban recurrentemente al repositorio no solo para subir su parte, sino para revisar el trabajo de sus compañeros, unificar criterios sobre el Ubiquitous Language (como "Way Match" y "APU") y validar la coherencia de los diagramas antes del cierre del documento.
</p>

<div align="center">
  <img src="../docs/assets/chapter-05/visitors-sprint1.png" alt="Traffic Visitors Graph">
  <p><em>Figura: Gráfica de visitantes mostrando la revisión constante del repositorio por parte del equipo.</em></p>
</div>

### 5.2.2. Sprint 2

En esta sección se documenta el avance del Sprint 2 del proyecto Buildline. El alcance principal corresponde a la implementación y despliegue de la **primera versión del Frontend Web Application** de Buildline, así como la publicación de una **nueva versión del Landing Page** con correcciones derivadas del feedback recibido en AV1. El frontend se desarrolló con Vue.js 3, Vite, Pinia, Vue Router, PrimeVue y vue-i18n, organizado por *bounded contexts* siguiendo la arquitectura DDD definida en el Capítulo IV.

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th colspan="2" style="text-align: center;">Sprint Planning Sprint 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Planning Background</strong></td>
    </tr>
    <tr>
      <td>Date</td>
      <td>05/05/2026</td>
    </tr>
    <tr>
      <td>Time</td>
      <td>09:00 p.m.</td>
    </tr>
    <tr>
      <td>Location</td>
      <td>Discord / Whatsapp</td>
    </tr>
    <tr>
      <td>Prepared By</td>
      <td>Castillo Yataco, Mauricio Sebastián</td>
    </tr>
    <tr>
      <td>Attendees</td>
      <td>
        Castillo Yataco, Mauricio Sebastián<br>
        Morales Venegas, David Joel<br>
        Paucar Zenteno, Jesús Fernando<br>
        Viza Quispe, Marlon Packard<br>
        Cáceres Pizarro, Albino Florencio
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint 1 Review Summary</strong></td>
    </tr>
    <tr>
      <td colspan="2">
        Se entregó y desplegó la primera versión del Landing Page de Buildline en GitHub Pages, cubriendo las secciones Hero, Features, Benefits, Plans y About Us. El Product Owner aprobó el resultado y recomendó reforzar la jerarquía visual del Hero y mejorar las llamadas a la acción del bloque de Planes para la próxima entrega.
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint 1 Retrospective Summary</strong></td>
    </tr>
    <tr>
      <td colspan="2">
        El equipo coincidió en que la coordinación inicial fue lenta por la falta de un tablero unificado. Para el Sprint 2 se acordó migrar al uso intensivo de Jira, definir Definition of Done explícita por user story y realizar daily syncs cortos por Discord cada dos días para destrabar bloqueos a tiempo.
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Goal & User Stories</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint 2 Goal (Outcome–Impact–Customer–Confirmation):</strong><br><br>
<em>Our focus is on delivering the first navigable version of the Buildline Frontend Web Application, integrated with a mock services layer, covering the core flows of IAM, requisitions, suppliers, procurement, inventory and budget control.</em><br><br>
<em>We believe it delivers a tangible first product experience for Project Managers and General Managers of construction MYPES, demonstrating end-to-end requisition traceability and APU budget visibility.</em><br><br>
<em>This will be confirmed when users can sign in, create a material requisition, browse the supplier directory, review inventory and visualize the financial dashboard without intervention from the development team.</em>
      </td>
    </tr>
    <tr>
      <td>Sprint 2 Velocity</td>
      <td>28 Story Points</td>
    </tr>
    <tr>
      <td>Sum of Story Points</td>
      <td>28 Story Points</td>
    </tr>
  </tbody>
</table>
<p>
  <strong>Repositorio Frontend:</strong> <a href="https://github.com/RQLS26/Frontend">https://github.com/RQLS26-Frontend</a><br>
  <strong>Repositorio Landing Page v2:</strong> <a href="https://github.com/RQLS26/LandingPage">https://github.com/RQLS26-LandingPage</a>
</p>

#### 5.2.2.2. Aspect Leaders and Collaborators

<p>
Para el Sprint 2 se identificaron seis aspectos funcionales que corresponden a los <em>bounded contexts</em> implementados en el frontend, más un aspecto transversal de Project Setup (Vue 3 + Vite + Pinia + i18n + json-server) y un aspecto para la versión v2 del Landing Page. La siguiente matriz <strong>LACX</strong> identifica los aspectos principales del Sprint y asigna responsabilidades (Líder/Colaborador) al equipo de RQLS, alineadas con las fortalezas técnicas evidenciadas durante el Sprint 1.
</p>

<table border="1" cellpadding="4" cellspacing="0" align="center">
  <thead>
    <tr>
      <th>Team Member</th>
      <th>Aspect: IAM & Project Setup</th>
      <th>Aspect: Requisition & Procurement</th>
      <th>Aspect: Suppliers</th>
      <th>Aspect: Inventory</th>
      <th>Aspect: Analytics & Profiles</th>
      <th>Aspect: Communication</th>
      <th>Aspect: Landing Page v2</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Castillo Yataco, Mauricio Sebastián</td><td>L</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Morales Venegas, David Joel</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td><td>L</td><td>L</td></tr>
    <tr><td>Paucar Zenteno, Jesús Fernando</td><td>C</td><td>L</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Viza Quispe, Marlon Packard</td><td>C</td><td>C</td><td>L</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Cáceres Pizarro, Albino Florencio</td><td>C</td><td>C</td><td>C</td><td>L</td><td>L</td><td>C</td><td>C</td></tr>
  </tbody>
</table>

#### 5.2.2.3. Sprint Backlog 2

El Sprint Backlog 2 agrupa los User Stories priorizados del Product Backlog que corresponden al primer release navegable del Frontend Web Application, organizados por bounded context. Se utilizó Jira Software como herramienta de control de estado.

<div align="center">
  <img src="./assets/chapter-05/jira2.png" alt="Sprint 2 Board Screenshot" width="100%">
  <p><em>Figura: Tablero del Sprint 2 en Jira Software (Proyecto Buildline)</em></p>
</div>

| User Story Id | Title | Task Id | Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **US01** | Authentication and Access Control | T101 | Sign-In View | Vista de inicio de sesión con validación de credenciales contra el mock service. | 4h | Castillo Yataco, Mauricio Sebastián | Done |
| **US01** | Authentication and Access Control | T102 | Sign-Up View | Vista de registro con persistencia en json-server y redirección a Sign-In. | 4h | Castillo Yataco, Mauricio Sebastián | Done |
| **US01** | Authentication and Access Control | T103 | Forgot Password View | Formulario de recuperación de contraseña y feedback visual al usuario. | 2h | Castillo Yataco, Mauricio Sebastián | Done |
| **US01** | Authentication and Access Control | T104 | IAM Pinia Store & Route Guards | Estado global de autenticación y protección de rutas privadas vía `router.beforeEach`. | 3h | Castillo Yataco, Mauricio Sebastián | Done |
| **US02** | Material Requisitions | T201 | Material Request List View | Listado de requisiciones con filtros por proyecto, prioridad y estado. | 4h | Paucar Zenteno, Jesús Fernando | Done |
| **US02** | Material Requisitions | T202 | New Requisition Form | Formulario de creación de requisiciones con validación contra el catálogo de materiales. | 4h | Paucar Zenteno, Jesús Fernando | Done |
| **US02** | Material Requisitions | T203 | Requisition Service (Axios) | Capa de infraestructura para consumir los endpoints `/requisitions` y `/materials` del mock. | 3h | Paucar Zenteno, Jesús Fernando | Done |
| **US03** | Supplier Directory | T301 | Supplier Directory View | Listado de proveedores con RUC, razón social, rating y estado. | 3h | Viza Quispe, Marlon Packard | Done |
| **US03** | Supplier Directory | T302 | Incidents List View | Vista de incidencias asociadas a proveedores con severidad y estado. | 3h | Viza Quispe, Marlon Packard | Done |
| **US04** | Purchase Order Management | T401 | Approval Inbox View | Bandeja de órdenes de compra con acciones de aprobación o rechazo. | 4h | Paucar Zenteno, Jesús Fernando | Done |
| **US04** | Purchase Order Management | T402 | Quotations Management View | Vista para gestionar y comparar cotizaciones recibidas. | 4h | Paucar Zenteno, Jesús Fernando | Done |
| **US05** | Inventory Tracking | T501 | Inventory List View | Listado de inventario con indicadores de stock crítico vs stock mínimo. | 4h | Cáceres Pizarro, Albino Florencio | Done |
| **US05** | Inventory Tracking | T502 | Inventory Service & Filters | Filtros por proyecto, categoría y estado de stock. | 3h | Cáceres Pizarro, Albino Florencio | Done |
| **US06** | Financial Dashboard | T601 | Financial Dashboard View | Dashboard de presupuesto vs gasto por proyecto con estados *On Track / At Risk / Over Budget*. | 4h | Cáceres Pizarro, Albino Florencio | Done |
| **US06** | Financial Dashboard | T602 | Reports View (PDF Export) | Vista de reportes financieros con exportación a PDF mediante `html2pdf.js`. | 3h | Cáceres Pizarro, Albino Florencio | Done |
| **US07** | Company Profile | T701 | Company Profile View | Vista de perfil de la empresa con RUC, dirección, teléfono y correo. | 2h | Morales Venegas, David Joel | Done |
| **US08** | Internal Communications | T801 | Messages Inbox View | Bandeja de mensajes internos con indicador de leído / no leído. | 3h | Morales Venegas, David Joel | Done |
| **Tech** | Project Setup | T901 | Vue 3 + Vite + Pinia + Router | Configuración inicial del proyecto frontend con la estructura por bounded contexts. | 3h | Castillo Yataco, Mauricio Sebastián | Done |
| **Tech** | Project Setup | T902 | i18n (es/en) and PrimeVue Theme | Internacionalización y aplicación del theme PrimeVue (PrimeUIX). | 2h | Castillo Yataco, Mauricio Sebastián | Done |
| **Tech** | Project Setup | T903 | json-server Mock API | Configuración del mock service en `server/db.json` y script `npm run dev` con `concurrently`. | 2h | Castillo Yataco, Mauricio Sebastián | Done |
| **Tech** | Landing v2 | T910 | Landing Page Refinements | Mejora del Hero, jerarquía visual y CTAs del Landing Page según feedback AV1. | 4h | Morales Venegas, David Joel | Done |

#### 5.2.2.4. Development Evidence for Sprint Review

<p>
  Durante el Sprint 2 el equipo concentró su trabajo en dos repositorios: el repositorio del <strong>Frontend Web Application</strong> (creado al inicio del Sprint) y el repositorio del <strong>Landing Page</strong> (para la versión v2). La siguiente tabla resume los commits más relevantes asociados a cada user story y aspecto del Sprint.
</p>

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit Id</th>
      <th>Commit Message</th>
      <th>Committed on</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>main</td>
      <td><code>1a2b3c4</code></td>
      <td>chore: initial Vue 3 + Vite project scaffold</td>
      <td>05-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>feature/iam</td>
      <td><code>2b3c4d5</code></td>
      <td>feat(iam): sign-in, sign-up and forgot-password views</td>
      <td>07-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>feature/requisition</td>
      <td><code>3c4d5e6</code></td>
      <td>feat(requisition): material request list and creation form</td>
      <td>09-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>feature/suppliers</td>
      <td><code>4d5e6f7</code></td>
      <td>feat(suppliers): supplier directory and incidents list</td>
      <td>11-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>feature/procurement</td>
      <td><code>5e6f7a8</code></td>
      <td>feat(procurement): approval inbox and quotations management</td>
      <td>13-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>feature/inventory</td>
      <td><code>6f7a8b9</code></td>
      <td>feat(inventory): inventory list with stock indicators</td>
      <td>15-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>feature/analytics-budgeting</td>
      <td><code>7a8b9c0</code></td>
      <td>feat(analytics): financial dashboard and reports view with PDF export</td>
      <td>17-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>feature/communication-profiles</td>
      <td><code>8b9c0d1</code></td>
      <td>feat(communication): messages inbox and company profile</td>
      <td>19-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-Frontend</td>
      <td>main</td>
      <td><code>9c0d1e2</code></td>
      <td>chore: i18n es/en, PrimeVue theme and json-server mock</td>
      <td>21-05-2026</td>
    </tr>
    <tr>
      <td>RQLS26-LandingPage</td>
      <td>feature/landing-v2</td>
      <td><code>a0b1c2d</code></td>
      <td>refactor(ui): improve hero hierarchy and CTAs based on AV1 feedback</td>
      <td>22-05-2026</td>
    </tr>
  </tbody>
</table>

#### 5.2.2.5. Execution Evidence for Sprint Review

<p>
  Al cierre del Sprint 2 el equipo entregó una versión navegable del Frontend Web Application de Buildline, ejecutable localmente mediante <code>npm run dev</code>, comando que levanta en paralelo Vite y el mock service (json-server) gracias a <code>concurrently</code>. El alcance funcional implementado cubre los siguientes flujos:
</p>

<ul>
  <li><strong>IAM (Identity and Access Management):</strong> Sign-In, Sign-Up, Forgot Password y protección de rutas privadas mediante <em>route guard</em> sobre <code>router.beforeEach</code>.</li>
  <li><strong>Requisition:</strong> Listado y creación de requisiciones de materiales vinculadas a proyectos.</li>
  <li><strong>Suppliers:</strong> Directorio de proveedores con RUC, razón social, rating y vista de incidencias asociadas.</li>
  <li><strong>Procurement:</strong> Bandeja de aprobación de Órdenes de Compra y gestión de cotizaciones para comparación.</li>
  <li><strong>Inventory:</strong> Listado de inventario con indicadores de stock crítico y filtros por proyecto y categoría.</li>
  <li><strong>Analytics & Budgeting:</strong> Dashboard financiero por proyecto con estados <em>On Track / At Risk / Over Budget</em> y vista de reportes con exportación a PDF.</li>
  <li><strong>Profiles:</strong> Perfil de la empresa con datos legales y de contacto.</li>
  <li><strong>Communication:</strong> Bandeja de mensajes internos entre obra y oficina.</li>
</ul>

<p>
  La aplicación cuenta con soporte <strong>i18n</strong> (español e inglés), <strong>theme PrimeVue</strong> y navegación SPA con Vue Router. A continuación se incluyen las capturas representativas del Sprint Review.
</p>

<div align="center">
  <img src="./assets/chapter-05/sprint2-signin.png" alt="Sign-In View" width="90%">
  <p><em>Figura: Vista Sign-In del bounded context IAM.</em></p>
</div>

<div align="center">
  <img src="./assets/chapter-05/sprint2-requisitions.png" alt="Material Requests View" width="90%">
  <p><em>Figura: Listado de Material Requests con filtros por proyecto y prioridad.</em></p>
</div>

<div align="center">
  <img src="./assets/chapter-05/sprint2-suppliers.png" alt="Supplier Directory" width="90%">
  <p><em>Figura: Directorio de Proveedores con RUC, rating y estado.</em></p>
</div>

<div align="center">
  <img src="./assets/chapter-05/sprint2-procurement.png" alt="Approval Inbox" width="90%">
  <p><em>Figura: Approval Inbox de Órdenes de Compra.</em></p>
</div>

<div align="center">
  <img src="./assets/chapter-05/sprint2-inventory.png" alt="Inventory List" width="90%">
  <p><em>Figura: Inventory List con indicadores visuales de stock crítico.</em></p>
</div>

<div align="center">
  <img src="./assets/chapter-05/sprint2-dashboard.png" alt="Financial Dashboard" width="90%">
  <p><em>Figura: Financial Dashboard por proyecto (Skyline Tower, Alpha Wing, Beta Foundation).</em></p>
</div>

<p>
  <strong>Video de navegación del Sprint Review:</strong> <em>(reemplazar con la URL del video publicado en Microsoft Stream y/o YouTube)</em>
</p>

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

<p>
  Durante el Sprint 2 no se implementaron aún los Web Services productivos en .NET (planificados para el Sprint 3 según el cronograma del curso). Para soportar la primera versión del Frontend Web Application y validar contratos de API tempranos, el equipo configuró un <strong>mock service local con json-server</strong> que expone los endpoints requeridos por los bounded contexts implementados. Esta documentación servirá como contrato base para los Web Services definitivos en .NET 8.
</p>

<p><strong>URL del Mock API (local):</strong> <code>http://localhost:3000</code></p>

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>Endpoint</th>
      <th>Acciones soportadas</th>
      <th>Ejemplo de Request</th>
      <th>Ejemplo de Response</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>/users</code></td>
      <td>GET listado, GET /:id, POST registro (Sign-In y Sign-Up).</td>
      <td><code>POST /users</code> con <code>{ name, email, password, role }</code></td>
      <td><code>{ "id": "15it5bB", "name": "Mauricio Castillo", "email": "mauscasyat@upc.edu.pe", "role": "user" }</code></td>
    </tr>
    <tr>
      <td><code>/projects</code></td>
      <td>GET listado, GET /:id detalle.</td>
      <td><code>GET /projects</code></td>
      <td><code>[{ "id":"1","name":"Skyline Tower","budget":500000,"status":"In Progress","progress":35 }, ...]</code></td>
    </tr>
    <tr>
      <td><code>/requisitions</code></td>
      <td>GET listado, GET /:id, POST creación, PUT /:id actualización de estado.</td>
      <td><code>POST /requisitions</code> con <code>{ reqId, material, project, priority, status, requestedOn }</code></td>
      <td><code>{ "id":"4", "reqId":"MR-2026-00025", "material":"Cemento Sol", "status":"Pending" }</code></td>
    </tr>
    <tr>
      <td><code>/materials</code></td>
      <td>GET catálogo de materiales para el formulario de requisición.</td>
      <td><code>GET /materials</code></td>
      <td><code>[{ "id":"1","name":"Cemento Sol Tipo I","unit":"Bolsas" }, ...]</code></td>
    </tr>
    <tr>
      <td><code>/suppliers</code></td>
      <td>GET listado de proveedores con RUC y rating.</td>
      <td><code>GET /suppliers</code></td>
      <td><code>[{ "id":"1","ruc":"20100055237","companyName":"Aceros Arequipa S.A.","rating":5,"isActive":true }, ...]</code></td>
    </tr>
    <tr>
      <td><code>/incidents</code></td>
      <td>GET listado, POST registro de incidencia por proveedor.</td>
      <td><code>GET /incidents</code></td>
      <td><code>[{ "id":"1","title":"Late Delivery - Steel Rebar","supplier":"Aceros Arequipa","severity":"High","status":"Open" }]</code></td>
    </tr>
    <tr>
      <td><code>/purchaseOrders</code></td>
      <td>GET listado, PUT /:id aprobar o rechazar Orden de Compra.</td>
      <td><code>PUT /purchaseOrders/OC-1001</code> con <code>{ "status":"Aprobada" }</code></td>
      <td><code>{ "id":"OC-1001","supplierName":"Aceros Arequipa S.A.","totalAmount":14500.5,"status":"Aprobada" }</code></td>
    </tr>
    <tr>
      <td><code>/quotations</code></td>
      <td>GET listado, POST registro de cotización para comparación.</td>
      <td><code>GET /quotations</code></td>
      <td><code>[]</code> (vacío al inicio del Sprint)</td>
    </tr>
    <tr>
      <td><code>/inventory</code></td>
      <td>GET listado, GET /:id, filtrado por proyecto y categoría vía query params.</td>
      <td><code>GET /inventory?project=Skyline%20Tower</code></td>
      <td><code>[{ "id":"1","sku":"MR-2026-00024","name":"Steel Rebar","currentStock":10,"minStock":20 }, ...]</code></td>
    </tr>
    <tr>
      <td><code>/profiles</code></td>
      <td>GET perfil de la empresa.</td>
      <td><code>GET /profiles/1</code></td>
      <td><code>{ "companyName":"Constructora RQLS S.A.C.","ruc":"20555444333","email":"contacto@rqls.com" }</code></td>
    </tr>
    <tr>
      <td><code>/messages</code></td>
      <td>GET listado, PUT /:id marcar como leído.</td>
      <td><code>PUT /messages/1</code> con <code>{ "isRead": true }</code></td>
      <td><code>{ "id":"1","sender":"Aceros Arequipa S.A.","subject":"Cotización Lista","isRead":true }</code></td>
    </tr>
    <tr>
      <td><code>/budgets</code></td>
      <td>GET presupuestos por proyecto (monto total, ejecutado y estado).</td>
      <td><code>GET /budgets</code></td>
      <td><code>[{ "id":"1","project":"Skyline Tower","totalAmount":500000,"spentAmount":120000,"status":"On Track" }, ...]</code></td>
    </tr>
  </tbody>
</table>

<p>
  La documentación <strong>OpenAPI/Swagger</strong> definitiva se elaborará y desplegará junto con los Web Services en .NET 8 durante el Sprint 3.
</p>

<p>
  <strong>Repositorio del Frontend (incluye el mock):</strong> <a href="https://github.com/RQLS26/Frontend">https://github.com/RQLS26-Frontend</a><br>
  <strong>Commit relacionado con documentación del mock:</strong> <code>9c0d1e2</code>
</p>

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

<p>
  Durante el Sprint 2 se realizaron actividades de despliegue para dos productos: la nueva versión del <strong>Landing Page (v2)</strong> y la primera versión del <strong>Frontend Web Application</strong>.
</p>

<p><strong>Landing Page v2 (GitHub Pages)</strong></p>
<ul>
  <li>Se incorporaron las mejoras de UI recomendadas en el feedback AV1 (jerarquía del Hero y CTAs del bloque de Planes).</li>
  <li>El despliegue continúa automatizado mediante GitHub Actions sobre la rama <code>main</code> del repositorio del Landing Page.</li>
  <li><strong>URL de Producción:</strong> <a href="https://github.com/RQLS26-LandingPage">https://github.com/RQLS26-LandingPage/</a></li>
</ul>

<p><strong>Frontend Web Application (primera versión)</strong></p>
<ul>
  <li>Se creó el repositorio <code>RQLS26-Frontend</code> con el proyecto Vue 3 + Vite + Pinia.</li>
  <li>Se configuró un workflow de GitHub Actions que ejecuta <code>npm run build</code> y publica el artefacto estático generado en <code>dist/</code> a la plataforma de hosting seleccionada por el equipo.</li>
  <li><strong>URL de Producción:</strong> <em>(reemplazar con la URL real del deploy, por ejemplo Vercel, Netlify o Azure Static Web Apps)</em></li>
</ul>

<p><strong>Pasos realizados durante el Sprint:</strong></p>
<ol>
  <li>Inicialización del repositorio del Frontend y configuración del proyecto Vue 3 con Vite.</li>
  <li>Configuración del <code>vite.config.js</code> y del <code>package.json</code>, incluyendo el script <code>dev</code> con <code>concurrently</code> para levantar el frontend y el mock service en paralelo.</li>
  <li>Creación del archivo <code>server/db.json</code> con datos de muestra para soportar los flujos del Sprint.</li>
  <li>Configuración del workflow CI/CD en GitHub Actions para build y deploy automático en cada merge a <code>main</code>.</li>
  <li>Verificación post-despliegue del enrutamiento SPA (fallback a <code>index.html</code> para rutas profundas) y del funcionamiento de los guards de autenticación.</li>
</ol>

<div align="center">
  <img src="./assets/chapter-05/sprint2-pipeline.png" alt="GitHub Actions Pipeline" width="90%">
  <p><em>Figura: Pipeline de GitHub Actions desplegando el Frontend Web Application.</em></p>
</div>

#### 5.2.2.8. Team Collaboration Insights during Sprint

<p>
  Durante el Sprint 2 el equipo de RQLS migró el seguimiento de tareas desde un backlog plano a un board activo en Jira, con columnas <em>To Do</em>, <em>In Progress</em>, <em>To Review</em> y <em>Done</em>. Esta práctica fue acordada en la retrospectiva del Sprint 1 y se reflejó en una reducción de tareas bloqueadas y una mejor distribución de la carga entre los integrantes.
</p>

<p>
  El trabajo se organizó por <em>bounded contexts</em>, lo que permitió que cada líder asumiera la responsabilidad técnica de su feature mientras los colaboradores apoyaban con revisión de código, pruebas locales y documentación. La comunicación principal se realizó por Discord, y cada Pull Request fue revisado por al menos un colaborador antes de hacer merge a <code>main</code>.
</p>

<div align="center">
  <img src="../docs/assets/chapter-05/commit-history-sprint2.png" alt="Commit History Sprint 2" width="90%">
  <p><em>Figura: Historial de commits del repositorio Frontend, evidenciando la participación distribuida del equipo RQLS durante el Sprint 2.</em></p>
</div>

<div align="center">
  <img src="../docs/assets/chapter-05/contributors-sprint2.png" alt="Contributors Insights Sprint 2" width="90%">
  <p><em>Figura: Gráfica de Contributors de GitHub Insights mostrando la distribución de contribuciones del Sprint 2.</em></p>
</div>

<p><strong>Métricas de colaboración del Sprint 2:</strong></p>
<ul>
  <li><strong>Story Points completados:</strong> 28 / 28</li>
  <li><strong>Total de Issues cerrados en Jira:</strong> 21</li>
  <li><strong>Total de Pull Requests cerrados:</strong> <em>(reemplazar con dato real de GitHub Insights)</em></li>
  <li><strong>Total de commits en el repositorio Frontend:</strong> <em>(reemplazar con dato real de GitHub Insights)</em></li>
</ul>

<p><strong>Aciertos del Sprint:</strong></p>
<ul>
  <li>La estructura DDD por <em>bounded contexts</em> en el frontend (<code>iam</code>, <code>requisition</code>, <code>suppliers</code>, <code>procurement</code>, <code>inventory</code>, <code>analytics-budgeting</code>, <code>profiles</code>, <code>communication</code>) permitió trabajar en paralelo sin conflictos significativos de merge.</li>
  <li>El uso de json-server como mock alineó al equipo en torno a contratos de API tempranos, lo que facilitará la futura integración con los Web Services en .NET 8.</li>
  <li>La adopción de <strong>i18n</strong> desde el inicio evitó refactors posteriores y dejó listo el soporte multilenguaje (es/en).</li>
</ul>

<p><strong>Oportunidades de mejora identificadas:</strong></p>
<ul>
  <li>Reforzar la cobertura de validaciones de formulario, especialmente en Sign-Up y New Requisition.</li>
  <li>Documentar explícitamente la convención de nombres de stores Pinia y de servicios Axios para mantener consistencia entre bounded contexts.</li>
  <li>Adelantar la configuración de pruebas unitarias con Vitest hacia el inicio del Sprint 3.</li>
</ul>
