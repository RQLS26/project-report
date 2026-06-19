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
      <td>Organización RQLS26</td>
      <td><a href="https://github.com/RQLS26">https://github.com/RQLS26</a></td>
    </tr>
    <tr>
      <td>Landing Page</td>
      <td><a href="https://github.com/RQLS26/buildline-landing-page">https://github.com/RQLS26/buildline-landing-page</a></td>
    </tr>
    <tr>
      <td>Frontend Web Application</td>
      <td><a href="https://github.com/RQLS26/buildline-frontend">https://github.com/RQLS26/buildline-frontend</a></td>
    </tr>
    <tr>
      <td>Backend Web Services</td>
      <td><a href="https://github.com/RQLS26/buildline-platform">https://github.com/RQLS26/buildline-platform</a></td>
    </tr>
  </tbody>
</table>

#### GitFlow Workflow and Collaboration Strategy
Para asegurar una colaboración organizada, evitar conflictos en el código y mantener la integración continua, el equipo RQLS aplica estrictamente **GitFlow** como flujo de trabajo de ramificación (Branching Workflow). La estrategia de colaboración se define de la siguiente manera:

* **main:** Rama que contiene el código de producción estable y auditado. Solo recibe integraciones a través de un proceso formal de Merge desde `release` o `hotfix`.
* **develop:** Rama de integración principal. Aquí se unifica el trabajo de los desarrolladores para preparar el próximo despliegue.
* **feature/&lt;módulo&gt;:** Ramas temporales creadas a partir de `develop` para aislar el desarrollo de nuevas Historias de Usuario (Ej: `feature/landing-hero-section`). La colaboración exige que estas ramas se integren a `develop` exclusivamente mediante **Pull Requests (PR)** en GitHub, requiriendo revisión de código (Code Review) antes de ser aprobadas.
* **hotfix/&lt;issue&gt;:** Ramas de corrección rápida creadas desde `main` para resolver bugs críticos o parches de emergencia.

El ciclo de vida del proyecto se apoya en Jira para asignar las tareas, asociando cada commit al ID de la tarea mediante Conventional Commits para una trazabilidad completa.


### 5.1.3. Source Code Style Guide & Conventions

En esta sección se establecen las convenciones de estilo y nomenclatura adoptadas para los lenguajes utilizados en el proyecto Buildline: HTML, CSS, JavaScript, TypeScript (Vue.js), C# (.NET 8) y Gherkin. Se aplica nomenclatura en inglés para todos los elementos del código, siguiendo el Ubiquitous Language definido para el dominio logístico de la construcción.

#### Referencias de Guías de Estilo Adoptadas

| Lenguaje/Tecnología | Guía de Estilo |
| :--- | :--- |
| HTML/CSS | [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html) |
| JavaScript | [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html) |
| TypeScript / Vue.js | [Vue.js Priority A Guide](https://vuejs.org/style-guide/rules-essential.html) |
| C# / .NET | [Microsoft C# Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions) |
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

#### Landing Page - Vercel
Despliegue automático del contenido estático mediante la integración con Vercel tras cada merge a la rama `main`.
* **URL:** [https://landing-page-bay-iota.vercel.app/](https://landing-page-bay-iota.vercel.app/)

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
  <strong>Repositorio:</strong> <a href="https://github.com/RQLS26/buildline-landing-page">https://github.com/RQLS26/buildline-landing-page</a>
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

Durante el Sprint 1, el equipo logró implementar con éxito el diseño, maquetación y despliegue de la Landing Page estática. A continuación, se presentan las evidencias visuales de la ejecución del producto de software, demostrando el cumplimiento de los Criterios de Aceptación de las Historias de Usuario planificadas:

**Evidencia 1: Hero Section y Propuesta de Valor**
Se desarrolló la pantalla de inicio principal destacando el mensaje de mitigación de sobrecostos y control del APU. La navegación superior es completamente funcional y el diseño respeta los lineamientos *responsive* para dispositivos móviles.
<div align="center">
  <img src="./assets/chapter-05/execution-hero.png" alt="Hero Section Evidence" width="90%">
  <p><em>Figura: Vista principal (Hero Section) desplegada en la Landing Page.</em></p>
</div>

**Evidencia 2: Sección de Beneficios y Trazabilidad**
Se maquetó la sección informativa donde se detallan los módulos de control de obra y aprobaciones jerárquicas, aplicando la paleta de colores corporativa y el sistema de diseño definido en Figma.
<div align="center">
  <img src="./assets/chapter-05/execution-benefits.png" alt="Benefits Section Evidence" width="90%">
  <p><em>Figura: Sección de características y propuesta de valor logístico.</em></p>
</div>

#### 5.2.1.6. Services Documentation Evidence
<p>
  Dado que el Sprint 1 abarca únicamente contenido estático (Landing Page de marketing), la implementación y consumo de la API en .NET para la gestión de requisiciones y órdenes de compra se abordará en los sprints posteriores orientados al Backend Web Services.
</p>

#### 5.2.1.7. Software Deployment Evidence
<p>
  <strong>URL de Producción:</strong> <a href="https://landing-page-bay-iota.vercel.app/">https://landing-page-bay-iota.vercel.app/</a>
</p>

#### 5.2.1.8. Team Collaboration Insights during Sprint

<p>
  Durante este primer sprint, el esfuerzo principal del equipo de RQLS se centró en la estructuración del proyecto, el diseño de UX/UI, la arquitectura de software y la elaboración de los requisitos técnicos (Capítulos I al IV). Por lo tanto, las evidencias de colaboración de GitHub presentadas a continuación corresponden al repositorio del <strong>Project Report</strong>, sentando las bases documentales y de diseño para la posterior codificación de la plataforma Buildline.
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
<em>Our focus is on delivering the first navigable version of the Buildline Frontend Web Application, integrated with a mock services layer, covering the core flows of IAM, requisitions, suppliers, procurement, delivery tracking, inventory and budget control.</em><br><br>
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
  <strong>Repositorio Frontend:</strong> <a href="https://github.com/RQLS26/buildline-frontend">https://github.com/RQLS26/buildline-frontend</a><br>
  <strong>Repositorio Landing Page v2:</strong> <a href="https://github.com/RQLS26/buildline-landing-page">https://github.com/RQLS26/buildline-landing-page</a>
</p>

#### 5.2.2.2. Aspect Leaders and Collaborators

<p>
Para el Sprint 2 se identificaron aspectos funcionales que corresponden a los <em>bounded contexts</em> implementados en el frontend, más un aspecto transversal de Project Setup (Vue 3 + Vite + Pinia + i18n + json-server) y un aspecto para la versión v2 del Landing Page. La siguiente matriz <strong>LACX</strong> identifica los aspectos principales del Sprint y asigna responsabilidades (Líder/Colaborador) al equipo de RQLS, alineadas con las fortalezas técnicas evidenciadas durante el Sprint 1.
</p>

<table border="1" cellpadding="4" cellspacing="0" align="center">
  <thead>
    <tr>
      <th>Team Member</th>
      <th>Aspect: IAM & Project Setup</th>
      <th>Aspect: Requisition & Procurement</th>
      <th>Aspect: Suppliers</th>
      <th>Aspect: Inventory & Delivery</th>
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
| **US11** | Delivery Tracking | T503 | Delivery Tracking View & Service | Vista y store para consultar entregas, crear registros de despacho y actualizar estados de entrega desde el mock `/deliveries`. | 4h | Cáceres Pizarro, Albino Florencio | Done |
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
      <td>buildline-frontend</td>
      <td>main</td>
      <td><code>1a2b3c4</code></td>
      <td>chore: initial Vue 3 + Vite project scaffold</td>
      <td>05-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
      <td>feature/iam</td>
      <td><code>2b3c4d5</code></td>
      <td>feat(iam): sign-in, sign-up and forgot-password views</td>
      <td>07-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
      <td>feature/requisition</td>
      <td><code>3c4d5e6</code></td>
      <td>feat(requisition): material request list and creation form</td>
      <td>09-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
      <td>feature/suppliers</td>
      <td><code>4d5e6f7</code></td>
      <td>feat(suppliers): supplier directory and incidents list</td>
      <td>11-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
      <td>feature/procurement</td>
      <td><code>5e6f7a8</code></td>
      <td>feat(procurement): approval inbox and quotations management</td>
      <td>13-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
      <td>feature/inventory</td>
      <td><code>6f7a8b9</code></td>
      <td>feat(inventory): inventory list with stock indicators</td>
      <td>15-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
      <td>feature/analytics-budgeting</td>
      <td><code>7a8b9c0</code></td>
      <td>feat(analytics): financial dashboard and reports view with PDF export</td>
      <td>17-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
      <td>feature/communication-profiles</td>
      <td><code>8b9c0d1</code></td>
      <td>feat(communication): messages inbox and company profile</td>
      <td>19-05-2026</td>
    </tr>
    <tr>
      <td>buildline-frontend</td>
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
  <li><strong>Delivery & Tracking:</strong> Seguimiento de entregas asociadas a órdenes de compra, con estados de despacho, tránsito, demora y entrega.</li>
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
  <p><em>Figura: Dashboard Overview (resumen).</em></p>
</div>

<h4>Video About The Product</h4>

<p>En esta sección se presenta el video demostrativo oficial de la plataforma <strong>Buildline (Release v1.0.0)</strong>, elaborado para el cierre del Sprint 2. El propósito de este video es evidenciar la integración end-to-end de nuestra arquitectura, mostrando desde la gestión de requisiciones y el control de inventario hasta el impacto automático en el Dashboard Financiero. El material audiovisual ha sido alojado de forma segura en la plataforma institucional <strong>Microsoft Stream</strong>.</p>

<div align="center">
  <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231b504_upc_edu_pe/IQBmp9aQwMuLSLxjirNLDL3-ATVaXbe2IUg_aTtw3V59494?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Y9T9qs" target="_blank">
    <img src="./assets/chapter-05/video-screenshot.png" alt="Video Demostrativo Buildline en Microsoft Stream" width="90%" style="border: 1px solid #ccc; border-radius: 8px;">
  </a>
  <p><em>Figura: Video demostrativo en Microsoft Stream.</em></p>
</div>

Enlace directo: https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231b504_upc_edu_pe/IQBmp9aQwMuLSLxjirNLDL3-ATVaXbe2IUg_aTtw3V59494?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Y9T9qs

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

<p>
  Durante el Sprint 2 no se implementaron aún los Web Services productivos en .NET (planificados para el Sprint 3 según el cronograma del curso). Para soportar la primera versión del Frontend Web Application y validar contratos de API tempranos, el equipo configuró un <strong>mock service local con json-server</strong> que expone los endpoints requeridos por los bounded contexts implementados. Esta documentación servirá como contrato base para los Web Services definitivos en .NET 8.
</p>

<p><strong>URL del Mock API (local):</strong> <code>http://localhost:3000</code></p>
<p><strong>URL del Mock API (Producción en Render):</strong> <code>https://buildline-json-server.onrender.com/</code></p>

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
    <tr>
      <td><code>/deliveries</code></td>
      <td>GET listado, GET /:id, POST creación y PATCH /:id actualización de estado de entrega.</td>
      <td><code>PATCH /deliveries/1</code> con <code>{ "status":"Delivered" }</code></td>
      <td><code>{ "id":"1","trackingId":"TRK-0048","purchaseOrder":"PO-2026-0015","status":"Delivered" }</code></td>
    </tr>
  </tbody>
</table>

<p>
  La documentación <strong>OpenAPI/Swagger</strong> definitiva se elaborará y desplegará junto con los Web Services en .NET 8 durante el Sprint 3.
</p>

<p>
  <strong>Repositorio del Frontend (incluye el mock):</strong> <a href="https://github.com/RQLS26/buildline-frontend">https://github.com/RQLS26/buildline-frontend</a><br>
  <strong>Commit relacionado con documentación del mock:</strong> <code>9c0d1e2</code>
</p>

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

<p>
  Durante el Sprint 2 se realizaron actividades de despliegue para dos productos: la nueva versión del <strong>Landing Page (v2)</strong> y la primera versión del <strong>Frontend Web Application</strong>.
</p>

<p><strong>Landing Page v2 (Vercel)</strong></p>
<ul>
  <li>Se incorporaron las mejoras de UI recomendadas en el feedback AV1 (jerarquía del Hero y CTAs del bloque de Planes).</li>
  <li>El despliegue fue migrado a la plataforma Vercel para asegurar integración nativa con Vite, automatizado en cada merge a <code>main</code>.</li>
  <li><strong>URL de Producción:</strong> <a href="https://landing-page-bay-iota.vercel.app/">https://landing-page-bay-iota.vercel.app/</a></li>
</ul>

<p><strong>Frontend Web Application (primera versión)</strong></p>
<ul>
  <li>Se actualizó el repositorio <code>buildline-frontend</code> con el proyecto Vue 3 + Vite + Pinia finalizado.</li>
  <li>Se configuró el despliegue automático conectando el repositorio directamente a <strong>Vercel</strong>, añadiendo el archivo <code>vercel.json</code> para manejar las reglas del Single Page Application (SPA).</li>
  <li>Se desplegó paralelamente el mock en <code>db.json</code> como un Web Service en <strong>Render</strong> para contar con persistencia remota.</li>
  <li><strong>URL de Producción:</strong> <a href="https://buildline-3jcvvnh4t-team-project0.vercel.app/">https://buildline-3jcvvnh4t-team-project0.vercel.app/</a></li>
</ul>

<p><strong>Pasos realizados durante el Sprint:</strong></p>
<ol>
  <li>Configuración del frontend dinámico utilizando variables de entorno (<code>VITE_API_BASE_URL</code>) para apuntar a Render en producción y localhost en desarrollo.</li>
  <li>Creación de un repositorio de backend para el `json-server` y despliegue a Render como servicio web.</li>
  <li>Conexión e importación del repositorio de Frontend a Vercel con la configuración de History Mode.</li>
  <li>Conexión de la Landing Page a Vercel, garantizando compatibilidad inmediata sin configuración adicional.</li>
  <li>Verificación exitosa post-despliegue del cruce de datos y navegación integral de ambas plataformas.</li>
</ol>

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
  <li><strong>Total de Issues cerrados en Jira:</strong> 22</li>
  <li><strong>Total de Pull Requests cerrados:</strong> 0</li>
  <li><strong>Total de commits en el repositorio Frontend:</strong> 20</li>
</ul>

<p><strong>Aciertos del Sprint:</strong></p>
<ul>
  <li>La estructura DDD por <em>bounded contexts</em> en el frontend (<code>iam</code>, <code>requisition</code>, <code>suppliers</code>, <code>procurement</code>, <code>inventory</code>, <code>delivery</code>, <code>analytics-budgeting</code>, <code>profiles</code>, <code>communication</code>) permitió trabajar en paralelo sin conflictos significativos de merge.</li>
  <li>El uso de json-server como mock alineó al equipo en torno a contratos de API tempranos, lo que facilitará la futura integración con los Web Services en .NET 8.</li>
  <li>La adopción de <strong>i18n</strong> desde el inicio evitó refactors posteriores y dejó listo el soporte multilenguaje (es/en).</li>
</ul>

<p><strong>Oportunidades de mejora identificadas:</strong></p>
<ul>
  <li>Reforzar la cobertura de validaciones de formulario, especialmente en Sign-Up y New Requisition.</li>
  <li>Documentar explícitamente la convención de nombres de stores Pinia y de servicios Axios para mantener consistencia entre bounded contexts.</li>
  <li>Adelantar la configuración de pruebas unitarias con Vitest hacia el inicio del Sprint 3.</li>
</ul>

### 5.2.3. Sprint 3

En esta sección se planifica el avance del Sprint 3 del proyecto Buildline. A diferencia del Sprint 1, centrado en la Landing Page, y del Sprint 2, centrado en la primera versión navegable del Frontend Web Application con mock API, el Sprint 3 se orienta a la primera versión de los **Backend Web Services** implementados con **ASP.NET Core / C#**.

Tras revisar el Sprint Backlog 1, el Sprint Backlog 2, las Technical Stories del Capítulo III, los diagramas de arquitectura del Capítulo IV y los endpoints consumidos por el Frontend local, se identificó que el backlog técnico anterior era demasiado limitado y estaba concentrado en perfiles/materiales. Por ello, el Sprint Backlog 3 toma como base Technical Stories de API granulares (`TS-IAM`, `TS-PROF`, `TS-SHARED`, `TS-REQ`, `TS-PROC`, `TS-INV`, `TS-DEL`, `TS-SUP`, `TS-ANB` y `TS-COM`) más mejoras transversales (`IMP-BE`) para foundation, persistencia y despliegue.

#### 5.2.3.1. Sprint Planning 3.

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th colspan="2" style="text-align: center;">Sprint Planning Sprint 3</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Planning Background</strong></td>
    </tr>
    <tr>
      <td>Date</td>
      <td>07/06/2026</td>
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
      <td>Morales Venegas, David Joel</td>
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
      <td colspan="2" style="text-align: center;"><strong>Sprint 2 Review Summary</strong></td>
    </tr>
    <tr>
      <td colspan="2">
        Se entregó la primera versión navegable del Frontend Web Application de Buildline, conectada a un mock API mediante json-server y organizada por bounded contexts. El equipo validó los flujos principales de autenticación, requisiciones, proveedores, compras, seguimiento de entregas, inventario, analítica, perfiles y comunicación.
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint 2 Retrospective Summary</strong></td>
    </tr>
    <tr>
      <td colspan="2">
        El uso del mock API permitió avanzar rápido en frontend, pero dejó como riesgo la falta de Web Services reales, persistencia transaccional y documentación Swagger definitiva. Para Sprint 3 se acordó priorizar la implementación de contratos backend compatibles con el frontend existente y mantener el tablero de Jira como fuente de seguimiento.
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Goal & User Stories</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint 3 Goal (Outcome-Impact-Customer-Confirmation):</strong><br><br>
<em>Our focus is on delivering the first functional version of Buildline Backend Web Services using ASP.NET Core / C#, replacing the mock services layer with REST endpoints aligned to the current Frontend Web Application contracts.</em><br><br>
<em>We believe it will reduce integration uncertainty for the development team and provide a deployable service foundation for construction MYPES that need secure, traceable requisition, procurement and inventory workflows.</em><br><br>
<em>This will be confirmed when Swagger exposes the prioritized API contracts, the frontend can consume the deployed backend for the selected flows, and the team can demonstrate authenticated access plus basic CRUD operations for the main bounded contexts.</em>
      </td>
    </tr>
    <tr>
      <td>Sprint 3 Velocity</td>
      <td>34 Story Points</td>
    </tr>
    <tr>
      <td>Sum of Story Points</td>
      <td>34 Story Points</td>
    </tr>
  </tbody>
</table>
<p>
  <strong>Repositorio Backend:</strong> <a href="https://github.com/RQLS26/buildline-platform">https://github.com/RQLS26/buildline-platform</a><br>
  <strong>Repositorio Frontend:</strong> <a href="https://github.com/RQLS26/buildline-frontend">https://github.com/RQLS26/buildline-frontend</a>
</p>

<p><strong>Planned backend branch evidence:</strong> las Technical Stories de API se trabajan con ramas por endpoint/flujo, por ejemplo <code>feature/TS-IAM-001-sign-in-api</code>, <code>feature/TS-IAM-002-sign-up-api</code>, <code>feature/TS-REQ-001-create-requisition-api</code>, <code>feature/TS-PROC-003-purchase-orders-api</code>, <code>feature/TS-INV-002-inventory-stock-update-api</code>, <code>feature/TS-DEL-002-delivery-status-update-api</code>, <code>feature/TS-SUP-003-incidents-api</code>, <code>feature/TS-ANB-001-budget-dashboard-api</code> y <code>feature/TS-COM-001-messages-inbox-api</code>. Las mejoras transversales se separan como <code>feature/backend-foundations</code>, <code>feature/backend-persistence-migrations</code> y <code>feature/backend-deployment-readiness</code>.</p>

#### 5.2.3.2. Aspect Leaders and Collaborators.

<p>
Para el Sprint 3 se identificaron aspectos backend alineados con los bounded contexts del diseño de arquitectura y con los nombres utilizados por el Frontend Web Application. `materials` y `categories` se mantienen como catálogos compartidos dentro de `shared`, no como bounded contexts principales independientes. La siguiente matriz <strong>LACX</strong> distribuye liderazgo y colaboración para equilibrar la carga técnica de la implementación en C#.
</p>

<table border="1" cellpadding="4" cellspacing="0" align="center">
  <thead>
    <tr>
      <th>Team Member</th>
      <th>Aspect: iam & security</th>
      <th>Aspect: profiles & shared catalog</th>
      <th>Aspect: requisition & procurement</th>
      <th>Aspect: inventory & delivery</th>
      <th>Aspect: suppliers & incidents</th>
      <th>Aspect: analytics-budgeting, communication & deployment</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Castillo Yataco, Mauricio Sebastián</td><td>L</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Morales Venegas, David Joel</td><td>C</td><td>L</td><td>C</td><td>C</td><td>C</td><td>L</td></tr>
    <tr><td>Paucar Zenteno, Jesús Fernando</td><td>C</td><td>C</td><td>L</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Viza Quispe, Marlon Packard</td><td>C</td><td>C</td><td>C</td><td>C</td><td>L</td><td>C</td></tr>
    <tr><td>Cáceres Pizarro, Albino Florencio</td><td>C</td><td>C</td><td>C</td><td>L</td><td>C</td><td>C</td></tr>
  </tbody>
</table>

#### 5.2.3.3. Sprint Backlog 3.

El Sprint Backlog 3 agrupa las tareas priorizadas para construir la primera versión de Web Services reales. La planificación respeta las Technical Stories actualizadas del Capítulo III y evita crear historias técnicas paralelas con nombres diferentes; cada work-item se vincula a TS de API concretas, orientadas a endpoints o flujos pequeños, y a las User Stories funcionales que justifican el contrato.

| Sprint # | User Story Id | User Story Title | Work-Item / Task Id | Work-Item / Task Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Sprint 3** | **IMP-BE-001** | Backend foundations | T300 | backend-foundations | Crear solución backend en C# con health check, CORS, JWT Bearer, Problem Details, XML documentation, Swagger auth y versionado `/api/v1`. | 5h | Castillo Yataco, Mauricio Sebastián | To-do |
| **Sprint 3** | **IMP-BE-002** | Persistence, migrations and seed data | T301 | backend-persistence-migrations | Configurar EF Core, DbContext, auditoría, constraints y seed data equivalente al mock `db.json` para los bounded contexts priorizados. | 6h | Morales Venegas, David Joel | To-do |
| **Sprint 3** | **TS-IAM-001 / TS-IAM-002 / US-022 / US-023** | Sign-in API / Sign-up API | T302 | iam authentication API | Implementar `POST /api/v1/auth/sign-in` y `POST /api/v1/auth/sign-up` con JWT, validaciones y respuestas compatibles con frontend. | 6h | Castillo Yataco, Mauricio Sebastián | To-do |
| **Sprint 3** | **TS-IAM-003 / TS-IAM-004 / TS-PROF-001 / US-024** | Users and profiles APIs | T303 | users-profiles API | Implementar `GET/POST /api/v1/users`, `GET/PATCH /api/v1/users/{id}` y lectura/actualización de `profiles`. | 6h | Castillo Yataco, Mauricio Sebastián | To-do |
| **Sprint 3** | **TS-SHARED-001 / TS-SHARED-002 / TS-SHARED-003 / US-004 / US-014** | Shared reference APIs | T304 | shared reference data API | Implementar `projects`, `materials` y `categories` como módulos de referencia dentro de `shared`, no como bounded contexts principales. | 5h | Morales Venegas, David Joel | To-do |
| **Sprint 3** | **TS-REQ-001 / TS-REQ-002 / TS-REQ-003 / US-001 / US-003 / US-004** | Requisition APIs | T305 | requisition API | Implementar creación, listado, detalle y actualización de `/api/v1/requisitions` con estado, prioridad, solicitante y proyecto. | 7h | Paucar Zenteno, Jesús Fernando | To-do |
| **Sprint 3** | **TS-PROC-001 / TS-PROC-002 / US-005 / US-006 / US-007** | Quotation APIs | T306 | quotations API | Implementar listado, creación, detalle y actualización de `/api/v1/quotations` para comparación de ofertas. | 5h | Paucar Zenteno, Jesús Fernando | To-do |
| **Sprint 3** | **TS-PROC-003 / TS-PROC-004 / US-008 / US-009 / US-016** | Purchase order APIs | T307 | purchase-orders API | Implementar listado, creación, detalle y actualización de `/api/v1/purchaseOrders` para compras aprobadas y trazabilidad. | 6h | Paucar Zenteno, Jesús Fernando | To-do |
| **Sprint 3** | **TS-INV-001 / TS-INV-002 / US-014 / US-015** | Inventory APIs | T308 | inventory API | Implementar listado, creación y actualización de stock en `/api/v1/inventory` con mínimos, máximos, proyecto y categoría. | 5h | Cáceres Pizarro, Albino Florencio | To-do |
| **Sprint 3** | **TS-DEL-001 / TS-DEL-002 / US-011 / US-012** | Delivery APIs | T309 | delivery API | Implementar listado, creación y actualización de entregas en `/api/v1/deliveries` con trackingId, proveedor, ETA y estado. | 5h | Cáceres Pizarro, Albino Florencio | To-do |
| **Sprint 3** | **TS-SUP-001 / TS-SUP-002 / US-029 / US-030** | Suppliers APIs | T310 | suppliers API | Implementar directorio, actualización y eliminación lógica de proveedores en `/api/v1/suppliers`. | 5h | Viza Quispe, Marlon Packard | To-do |
| **Sprint 3** | **TS-SUP-003 / TS-SUP-004 / US-013** | Incidents APIs | T311 | incidents API | Implementar creación, listado y actualización de incidencias en `/api/v1/incidents` con severidad, estado, proveedor y orden asociada. | 4h | Viza Quispe, Marlon Packard | To-do |
| **Sprint 3** | **TS-ANB-001 / TS-ANB-002 / US-017 / US-018 / US-019** | Budget APIs | T312 | analytics-budgeting API | Implementar lectura y actualización de `/api/v1/budgets` con totalBudget, spent, allocated y estados presupuestales. | 4h | Morales Venegas, David Joel | To-do |
| **Sprint 3** | **TS-COM-001 / TS-COM-002 / US-010 / US-021** | Messages APIs | T313 | communication API | Implementar bandeja, creación, actualización y eliminación de `/api/v1/messages` para alertas y mensajes internos. | 4h | Viza Quispe, Marlon Packard | To-do |
| **Sprint 3** | **IMP-BE-003** | Deployment and integration readiness | T314 | backend-deployment-readiness | Preparar Docker, configuración de producción, variables de entorno, ejemplos HTTP y smoke test con frontend reemplazando json-server. | 5h | Morales Venegas, David Joel | To-do |

<p><strong>Endpoint coverage planned for Sprint 3:</strong> <code>/api/v1/auth/sign-in</code>, <code>/api/v1/auth/sign-up</code>, <code>/api/v1/users</code>, <code>/api/v1/profiles</code>, <code>/api/v1/projects</code>, <code>/api/v1/materials</code>, <code>/api/v1/categories</code>, <code>/api/v1/requisitions</code>, <code>/api/v1/quotations</code>, <code>/api/v1/purchaseOrders</code>, <code>/api/v1/inventory</code>, <code>/api/v1/deliveries</code>, <code>/api/v1/suppliers</code>, <code>/api/v1/incidents</code>, <code>/api/v1/budgets</code> y <code>/api/v1/messages</code>.</p>

#### 5.2.3.4. Development Evidence for Sprint Review

<p>
En esta sección se explican y presentan los avances en la implementación logrados durante el Sprint 3 en relación con los <strong>Backend Web Services</strong> de Buildline. A lo largo de este sprint se construyó la primera versión real de la API REST utilizando <strong>ASP.NET Core 8 / C#</strong>, reemplazando el mock service con una arquitectura robusta estructurada por Bounded Contexts, persistencia mediante Entity Framework Core y seguridad con JWT Bearer.
</p>

<p>
La tabla siguiente resume los commits más relevantes realizados en el repositorio del Backend, indicando la rama, el mensaje asociado, una breve descripción del cambio introducido y la fecha de commit.
</p>

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit Message</th>
      <th>Commit Message Body</th>
      <th>Committed on (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="12">
        <a href="https://github.com/RQLS26/buildline-platform">
          buildline-platform
        </a>
      </td>
      <td>feature/backend-foundations</td>
      <td>feat(core): initial ASP.NET Core 8 Web API scaffold</td>
      <td>Crea la solución base en C#, configurando CORS, Swagger, Problem Details y la estructura de carpetas por Bounded Contexts.</td>
      <td>08-06-2026</td>
    </tr>
    <tr>
      <td>feature/backend-persistence</td>
      <td>feat(data): setup EF Core DbContext and base entities</td>
      <td>Configura Entity Framework Core, agrega interfaces base (IAuditableEntity) y genera la migración inicial de la base de datos.</td>
      <td>09-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-IAM-001-auth</td>
      <td>feat(iam): implement JWT authentication and AuthController</td>
      <td>Implementa lógica de generación de tokens JWT, hashing de contraseñas (BCrypt) y endpoints de Sign-In y Sign-Up.</td>
      <td>10-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-PROF-001-profiles</td>
      <td>feat(profiles): add profiles endpoints and facade</td>
      <td>Crea controladores y servicios para gestionar perfiles y exponer el ProfilesContextFacade.</td>
      <td>11-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-REQ-001-requisition</td>
      <td>feat(requisition): implement RequisitionsController and logic</td>
      <td>Desarrolla el flujo completo para crear, listar y actualizar requisiciones y materiales asociados a proyectos.</td>
      <td>12-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-PROC-003-procurement</td>
      <td>feat(procurement): add purchase orders and quotations endpoints</td>
      <td>Implementa la gestión de órdenes de compra y cotizaciones con sus respectivos eventos de dominio (cambios de estado).</td>
      <td>13-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-INV-002-inventory</td>
      <td>feat(inventory): implement inventory stock tracking</td>
      <td>Crea los servicios para consultar inventario por categoría y registrar eventos de cambio de stock (StockLevel).</td>
      <td>14-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-DEL-002-delivery</td>
      <td>feat(delivery): add delivery tracking management</td>
      <td>Agrega endpoints para registrar despachos, códigos de seguimiento (TrackingCode) y modificar estados de entregas.</td>
      <td>15-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-SUP-001-suppliers</td>
      <td>feat(suppliers): implement supplier directory and incidents</td>
      <td>Desarrolla la gestión de proveedores, calificaciones (SupplierRating) y el registro de incidencias asociadas.</td>
      <td>15-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-ANB-001-analytics</td>
      <td>feat(analytics): implement budget calculations API</td>
      <td>Agrega lógica financiera para evaluar la salud del presupuesto (BudgetHealth) y exponerlo al dashboard analítico.</td>
      <td>16-06-2026</td>
    </tr>
    <tr>
      <td>feature/TS-COM-001-messages</td>
      <td>feat(communication): add internal messages API</td>
      <td>Implementa bandeja de entrada (InboxState) y lógica para enviar comunicaciones internas y gestionar su estado.</td>
      <td>17-06-2026</td>
    </tr>
    <tr>
      <td>feature/backend-deployment</td>
      <td>build(deploy): prepare Dockerfile and appsettings</td>
      <td>Configura el Dockerfile, docker-compose.yml y los appsettings de producción para el despliegue del API.</td>
      <td>18-06-2026</td>
    </tr>
  </tbody>
</table>

#### 5.2.3.5. Execution Evidence for Sprint Review

<p>
Durante el Sprint 3 se consolidó la transición del entorno simulado (mock) a un entorno backend transaccional real. La principal evidencia de ejecución se manifiesta en la correcta inicialización del proyecto ASP.NET Core, la conexión a la base de datos mediante Entity Framework y la ejecución de la interfaz de pruebas automatizada autogenerada.
</p>

<p>A continuación, se presentan las capturas representativas de la plataforma operativa a nivel de servicios:</p>

<div align="center">
  <img src="./assets/chapter-05/sprint3-swagger-ui.png" alt="Swagger UI Execution Evidence" width="90%">
  <p><em>Figura: Interfaz de Swagger UI generada automáticamente por ASP.NET Core, listando y documentando los endpoints V1 de los Bounded Contexts desarrollados (IAM, Procurement, Inventory, etc.).</em></p>
</div>

<div align="center">
  <img src="./assets/chapter-05/sprint3-postman-test.png" alt="Postman Request Evidence" width="90%">
  <p><em>Figura: Prueba de ejecución exitosa (HTTP 200 OK) de un endpoint seguro utilizando el token JWT Bearer desde un cliente REST (ej. Postman).</em></p>
</div>

#### 5.2.3.6. Services Documentation Evidence for Sprint Review

<p>
En el Sprint 3, la documentación de servicios evolucionó a un contrato formal e interactivo. Buildline ahora emplea <strong>Swagger / OpenAPI 3.0</strong>, configurado nativamente en ASP.NET Core. Este contrato sirve como única fuente de verdad para la integración con el Frontend.
</p>
<p>
La tabla a continuación detalla los contratos de los servicios RESTful habilitados en la versión actual:
</p>

<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>Endpoint Base</th>
      <th>Método HTTP</th>
      <th>Descripción del Servicio</th>
      <th>Request Payload / Params</th>
      <th>Response Típico (Código)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2"><strong>/api/v1/authentication</strong></td>
      <td><code>POST</code></td>
      <td><strong>Sign-In:</strong> Valida credenciales y retorna un token JWT.</td>
      <td><code>{ "email", "password" }</code></td>
      <td><code>200 OK</code>: Token y datos de sesión.</td>
    </tr>
    <tr>
      <td><code>POST</code></td>
      <td><strong>Sign-Up:</strong> Crea un nuevo usuario y cifra la contraseña.</td>
      <td><code>{ "firstName", "lastName", "email", "password" }</code></td>
      <td><code>201 Created</code>: Mensaje de éxito.</td>
    </tr>
    <tr>
      <td rowspan="2"><strong>/api/v1/requisitions</strong></td>
      <td><code>GET</code></td>
      <td>Lista todas las requisiciones filtradas por proyecto.</td>
      <td>Query param: <code>?projectId=1</code></td>
      <td><code>200 OK</code>: Lista de DTOs Requisition.</td>
    </tr>
    <tr>
      <td><code>POST</code></td>
      <td>Crea una nueva solicitud de materiales para la obra.</td>
      <td><code>{ "projectId", "materialId", "priority" }</code></td>
      <td><code>201 Created</code>: ID de la requisición.</td>
    </tr>
    <tr>
      <td rowspan="2"><strong>/api/v1/purchaseOrders</strong></td>
      <td><code>GET</code></td>
      <td>Obtiene la bandeja de entrada de órdenes de compra pendientes.</td>
      <td>-</td>
      <td><code>200 OK</code>: Arreglo de órdenes de compra.</td>
    </tr>
    <tr>
      <td><code>PUT</code></td>
      <td>Actualiza el estado (Aprobado/Rechazado) de la orden.</td>
      <td><code>{ "status": "Approved" }</code></td>
      <td><code>200 OK</code>: Orden de compra actualizada.</td>
    </tr>
    <tr>
      <td rowspan="2"><strong>/api/v1/inventory</strong></td>
      <td><code>GET</code></td>
      <td>Obtiene el inventario actual de materiales.</td>
      <td>Query param: <code>?categoryId=2</code></td>
      <td><code>200 OK</code>: Datos de stock actual vs mínimos.</td>
    </tr>
    <tr>
      <td><code>POST</code></td>
      <td>Registra entradas/salidas de almacén.</td>
      <td><code>{ "materialId", "quantity", "type" }</code></td>
      <td><code>200 OK</code>: Nuevo balance de stock.</td>
    </tr>
    <tr>
      <td><strong>/api/v1/suppliers</strong></td>
      <td><code>GET</code></td>
      <td>Directorio de proveedores activos y su calificación.</td>
      <td>-</td>
      <td><code>200 OK</code>: Lista de proveedores.</td>
    </tr>
    <tr>
      <td><strong>/api/v1/budgets</strong></td>
      <td><code>GET</code></td>
      <td>Métricas financieras: Gastos vs Presupuesto Total.</td>
      <td>Query param: <code>?projectId=1</code></td>
      <td><code>200 OK</code>: KPIs financieros (BudgetHealth).</td>
    </tr>
  </tbody>
</table>

#### 5.2.3.7. Software Deployment Evidence for Sprint Review

<p>
Para garantizar el acceso público y concurrente por parte del equipo Frontend y facilitar las pruebas de integración, los Backend Web Services fueron contenerizados mediante Docker y desplegados en un entorno en la nube.
</p>

<p><strong>Configuración de Producción:</strong></p>
<ul>
  <li>Se utilizó el <code>Dockerfile</code> definido en la raíz del proyecto para construir la imagen del API en .NET 8.</li>
  <li>Las migraciones de Entity Framework fueron aplicadas a la base de datos de producción para generar el esquema de tablas actualizado.</li>
  <li>Se configuraron variables de entorno críticas y secretos (como la cadena de conexión y la llave secreta JWT) directamente en los ajustes (<code>appsettings.Production.json</code> / Variables de entorno del servidor).</li>
</ul>

<div align="center">
  <img src="./assets/chapter-05/sprint3-deployment-evidence.png" alt="Backend Deployment Evidence" width="90%">
  <p><em>Figura: Panel de control del entorno de nube evidenciando el estado de ejecución (Running) del contenedor del servicio Web API de Buildline.</em></p>
</div>

#### 5.2.3.8. Team Collaboration Insights during Sprint

<p>
Durante el Sprint 3, la dinámica de trabajo del equipo se adaptó a las necesidades técnicas del proyecto. Dado que el esfuerzo principal fue la creación de la arquitectura Backend desde cero utilizando C# y ASP.NET Core, los <em>commits</em> en el repositorio <code>buildline-platform</code> fueron realizados principalmente por los desarrolladores asignados específicamente a esta capa lógica.
</p>

<p>
Esta centralización de los <em>commits</em> en el repositorio no implica una falta de colaboración, sino una <strong>división estratégica de roles funcionales</strong>. Mientras los encargados del Backend implementaban los controladores, repositorios y la seguridad JWT, el resto del equipo se enfocó en tareas transversales críticas para el éxito del sprint:
</p>

<ul>
  <li><strong>Integración Frontend:</strong> Adaptación de las llamadas Axios en la aplicación Vue.js para consumir los nuevos endpoints reales en lugar del mock server.</li>
  <li><strong>Diseño y Modelado:</strong> Estructuración del diagrama de base de datos relacional que guio la creación de las entidades en Entity Framework Core.</li>
  <li><strong>Aseguramiento de Calidad (QA):</strong> Pruebas manuales exhaustivas de las rutas de la API a través de Postman y Swagger.</li>
  <li><strong>Documentación y Despliegue:</strong> Preparación del entorno Docker y redacción técnica de los reportes del proyecto.</li>
</ul>

<div align="center">
  <img src="../docs/assets/chapter-05/sprint3-network-graph.png" alt="Network Graph Sprint 3" width="90%">
  <p><em>Figura: Network Graph del repositorio evidenciando la estructura de ramas (GitFlow) utilizada para aislar el desarrollo de cada Bounded Context antes de su integración.</em></p>
</div>

<p><strong>Aciertos del Sprint 3:</strong></p>
<ul>
  <li>La correcta separación en Bounded Contexts (IAM, Procurement, Inventory, etc.) permitió tener un código altamente modular, facilitando el mantenimiento y evitando conflictos graves al momento de fusionar ramas.</li>
  <li>La especialización de roles permitió avanzar en paralelo en el despliegue de la API, las pruebas del Frontend y la documentación, sin generar cuellos de botella.</li>
</ul>

<p><strong>Oportunidades de mejora identificadas:</strong></p>
<ul>
  <li>Será beneficioso implementar un sistema de CI/CD automatizado (ej. GitHub Actions) que integre pruebas unitarias para cada <em>Pull Request</em> antes de llegar a la rama principal.</li>
</ul>
