
<div align="center">
<br>
<img src="docs/assets/common/logo-upc.png"
width="180" alt="Logo UPC">
<br><br>

# UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS {-}

<br>

### Facultad de Ingeniería
### Carrera de Ingeniería de Software

<br>

**Ciclo Académico 2026-10**

<br>

**Código:** 1ASI0730 &nbsp; | &nbsp; **Curso:** Aplicaciones Web &nbsp; | &nbsp; **NRC:** 12158

<br>

**Docente:** Villafuerte Bazan, Oscar Ivan

<br>

# Informe de Trabajo Final - AV1 {-}

<br>

### **Nombre de la Startup:**
**RQLS (Requisitions, Quotes, Logistics System)**

<br>

### **Nombre del Producto:**
**Buildline**

<br>

### Relación de integrantes

<table align="center" style="margin: 0 auto; font-size: 15px;">
<thead>
    <tr>
      <th align="center">Código</th>
      <th align="center">Apellidos y Nombres</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">U202113229</td>
      <td align="left">Castillo Yataco, Mauricio Sebastián</td>
    </tr>
    <tr>
      <td align="center">U20231B504</td>
      <td align="left">Morales Venegas, David Joel</td>
    </tr>
    <tr>
      <td align="center">U202316687</td>
      <td align="left">Paucar Zenteno, Jesús Fernando</td>
    </tr>
    <tr>
      <td align="center">U202322849</td>
      <td align="left">Viza Quispe, Marlon Packard</td>
    </tr>
    <tr>
      <td align="center">U201923820</td>
      <td align="left">Cáceres Pizarro, Albino Florencio</td>
    </tr>
  </tbody>
</table>

<br><br>

**Lima, abril de 2026**
</div>

# Registro de versiones del informe {-}
| Versión | Fecha | Autores | Descripción |
| :--- | :--- | :--- | :--- |
| 1.0.0 | 26/04/2026 | Mauricio Sebastián Castillo Yataco, David Joel Morales Venegas, Jesús Fernando Paucar Zenteno, Marlon Packard Viza Quispe, Albino Florencio Cáceres Pizarro | Versión inicial del avance AV1 (TB1) |
| 2.0.0 | 16/05/2026 | Mauricio Sebastián Castillo Yataco, David Joel Morales Venegas, Jesús Fernando Paucar Zenteno, Marlon Packard Viza Quispe, Albino Florencio Cáceres Pizarro | Implementación del Sprint 2: Frontend Web Application funcional con módulos IAM, Requisition, Procurement, Inventory, Analytics & Budgeting, navegación SPA e i18n |


# Project Report Collaboration Insights
El presente apartado tiene como finalidad evidenciar el trabajo colaborativo realizado durante el desarrollo del informe. Para ello, se pone a disposición el repositorio oficial del proyecto, alojado en una organización pública de GitHub:

🔗 https://github.com/RQLS26

A partir de este repositorio, se analiza la participación de los integrantes del equipo mediante indicadores como número de commits, frecuencia de contribuciones y actividad general registrada en la plataforma.

En el contexto de la entrega correspondiente a la TB1, TP1, TB2 y TF1, se presenta un análisis de colaboración que permite visualizar el nivel de aporte individual de cada miembro del equipo, sustentado en los registros de GitHub. Este análisis busca demostrar la distribución del trabajo, la constancia en el desarrollo del informe y el cumplimiento de las actividades asignadas.

## TB1
[pending content]

## TP1
[pending content]

## TB2
[pending content]

## TF1
[pending content]


# Contenido {-}
## Tabla de contenidos {-}

- [Carátula](#informe-de-trabajo-final---av1)
- [Registro de Versiones del Informe](#registro-de-versiones-del-informe)
- [Student Outcome](#student-outcome)
- [Abstract](#abstract)
- [Resumen](#resumen)

- [Capítulo I: Introducción](#capítulo-i-introducción)
    - [1.1. Startup Profile](#11-startup-profile)
    - [1.2. Solution Profile](#12-solution-profile)
    - [1.3. Segmentos objetivo](#13-segmentos-objetivo)

- [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
    - [2.1. Competidores](#21-competidores)
    - [2.2. Entrevistas](#22-entrevistas)
    - [2.3. Needfinding](#23-needfinding)
    - [2.4. Big Picture EventStorming](#24-big-picture-eventstorming)
    - [2.5. Ubiquitous Language](#25-ubiquitous-language)

- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
    - [3.1. User Stories](#31-user-stories)
    - [3.2. Impact Mapping](#32-impact-mapping)
    - [3.3. Product Backlog](#33-product-backlog)

- [Capítulo IV: Product Design](#capítulo-iv-product-design)
    - [4.1. Style Guidelines](#41-style-guidelines)
    - [4.2. Information Architecture](#42-information-architecture)
    - [4.3. Landing Page UI Design](#43-landing-page-ui-design)
    - [4.4. Web Applications UX/UI Design](#44-web-applications-uxui-design)
    - [4.5. Web Applications Prototyping](#45-web-applications-prototyping)
    - [4.6. Domain-Driven Software Architecture](#46-domain-driven-software-architecture)
    - [4.7. Software Object-Oriented Design](#47-software-object-oriented-design)
    - [4.8. Database Design](#48-database-design)

- [Capítulo V: Product Implementation, Validation & Deployment](#capítulo-v-product-implementation-validation--deployment)
    - [5.1. Software Configuration Management](#51-software-configuration-management)
    - [5.2. Landing Page, Services & Applications Implementation](#52-landing-page-services--applications-implementation)
    - [5.3. Validation Interviews](#53-validation-interviews)
    - [5.4. Video About-the-Product](#54-video-about-the-product)

- [Capítulo VI: Conclusions](#capítulo-vi-conclusions)
    - [6.1. Conclusiones y recomendaciones](#61-conclusiones-y-recomendaciones)
    - [6.2. Video About-the-Team](#62-video-about-the-team)

- [Bibliografía](#bibliografía)

# Student Outcome {-}
El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET – EAC - Student Outcome 5**  
**Criterio:** La capacidad de funcionar efectivamente en un equipo cuyos miembros juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo, establecen objetivos, planifican tareas y cumplen objetivos.

En el siguiente cuadro se describen las acciones realizadas y las conclusiones del equipo, que permiten sustentar el logro del ABET – EAC - Student Outcome 5.

---

## Tabla de Student Outcome
<table style="width:100%; border-collapse: collapse;">
  <tr>
    <th style="width:25%;">Criterio específico</th>
    <th style="width:45%;">Acciones realizadas</th>
    <th style="width:30%;">Conclusiones</th>
  </tr>

  <tr>
    <td>
      Trabaja en equipo para proporcionar liderazgo en forma conjunta
    </td>
    <td>
      <strong>Morales Venegas, David Joel</strong> — Creación del repositorio, Diseño de Landing Page, Lideró diseño/análisis de entrevistas.<br>
      <strong>Viza Quispe, Marlon Packard</strong> — Event Storming, Ubiquitous Language, Journey/Empathy Mapping.<br>
      <strong>Paucar Zenteno, Jesús Fernando</strong> — User Flow Diagrams, Web applications prototype.<br>
      <strong>Castillo Yataco, Mauricio Sebastián</strong> — Lean UX Process, Segmentos Objetivo, Lean UX Canvas, Needfinding.<br>
      <strong>Cáceres Pizarro, Albino Florencio</strong> — Arquitectura de software (C4 Context Diagrams y Class Diagrams).<br>
    </td>
    <td>
      <strong>AV1:</strong> El equipo demostró liderazgo compartido al asignar responsables específicos basándose en las fortalezas técnicas de cada integrante.<br>
      <strong>TB1:</strong> Se establecieron metas claras para el descubrimiento de usuarios, logrando una visión holística del problema logístico.<br>
    </td>
  </tr>
  <tr>
    <td>
      Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos
    </td>
    <td>
      <strong>Morales Venegas, David Joel</strong> — Colaboró en Wireframes, Wireflow y User Flow Diagrams.<br>
      <strong>Viza Quispe, Marlon Packard</strong> — Diseño de Landing Page, revisión integradora y correcciones finales AV1.<br>
      <strong>Paucar Zenteno, Jesús Fernando</strong> — Diseño de Web Applications, revisión integradora y correcciones finales AV1.<br>
      <strong>Castillo Yataco, Mauricio Sebastián</strong> — Diseño de arquitectura, Redacción y documentación del Capítulo V (SCM, Sprint 1).<br>
      <strong>Cáceres Pizarro, Albino Florencio</strong> — Análisis de competidores, diagrama de base de datos y artefactos de Needfinding.<br>
    </td>
    <td>
      <strong>AV1:</strong> La planificación de tareas mediante un backlog inicial permitió cumplir con todos los artefactos de Needfinding y Lean UX.<br>
      <strong>TB1:</strong> El entorno colaborativo en GitHub facilitó la integración de los diagramas de arquitectura y el prototipo inicial.<br>
    </td>
  </tr>
</table>


# Abstract
This project addresses the operational inefficiencies and digital gap within micro and small enterprises (MSMEs) in the Peruvian construction sector. Focusing on the procurement and logistics chain, the development follows the Lean UX framework and Agile methodologies to design a specialized Software as a Service (SaaS) platform. The system centralizes requisitions, quotation comparisons, and multi-level approval workflows to replace informal communication channels. Preliminary research and user discovery suggest that the implementation of such a solution significantly improves budget traceability and reduces administrative lead times. Ultimately, this work contributes to the digital maturity of the industry by providing an accessible tool for operational optimization.

# Resumen
Este proyecto aborda las ineficiencias operativas y la brecha digital en las micro y pequeñas empresas (MYPES) del sector construcción en el Perú. Centrándose en la cadena de adquisiciones y logística, el desarrollo sigue el marco de trabajo Lean UX y metodologías ágiles para diseñar una plataforma especializada bajo el modelo Software as a Service (SaaS). El sistema centraliza las requisiciones, la comparativa de cotizaciones y los flujos de aprobación multinivel para reemplazar los canales de comunicación informales. La investigación preliminar y el descubrimiento de usuarios sugieren que la implementación de una solución de este tipo mejora significativamente la trazabilidad presupuestal y reduce los tiempos de espera administrativos. En última instancia, este trabajo contribuye a la madurez digital de la industria al proporcionar una herramienta accesible para la optimización operativa


# Buildline - Project Report (RQLS)

Este repositorio contiene la documentación técnica y el informe detallado del proyecto **Buildline**, desarrollado por la startup **RQLS** para el curso de Aplicaciones Web.

## 📂 Estructura del Repositorio
*   `/docs`: Contiene los archivos Markdown individuales del informe (Capítulos I - VI).
*   `/docs/front-matter`: Carátula, registro de versiones, TOC y resúmenes.
*   `/docs/assets`: Recursos visuales, diagramas de arquitectura y evidencias de Sprint.

## 🔗 Enlaces de Interés
*   **Organización GitHub**: [https://github.com/RQLS26](https://github.com/RQLS26)
*   **Repositorio Landing Page**: [https://github.com/RQLS26/Landing-Page](https://github.com/RQLS26/Landing-Page)

---
© 2026 RQLS Team - Universidad Peruana de Ciencias Aplicadas
Documentación inicial del proyecto:

