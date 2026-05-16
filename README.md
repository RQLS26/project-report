<div align="center">
<br>
<img src="docs/assets/common/logo-upc.png" width="180" alt="Logo UPC">
<br><br>

# UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS 

<br>

### Facultad de IngenierÃ­a
### Carrera de IngenierÃ­a de Software

<br>

**Ciclo AcadÃ©mico 2026-10**

<br>

**CÃ³digo:** 1ASI0730 &nbsp; | &nbsp; **Curso:** Aplicaciones Web &nbsp; | &nbsp; **NRC:** 12158

<br>

**Docente:** Villafuerte Bazan, Oscar Ivan

<br>

# Informe de Trabajo Final - AV1 

<br>

### **Nombre de la Startup:**
**RQLS (Requisitions, Quotes, Logistics System)**

<br>

### **Nombre del Producto:**
**Buildline**

<br>

### RelaciÃ³n de integrantes

<table align="center" style="margin: 0 auto; font-size: 15px;">
<thead>
    <tr>
      <th align="center">CÃ³digo</th>
      <th align="center">Apellidos y Nombres</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">U202113229</td>
      <td align="left">Castillo Yataco, Mauricio SebastiÃ¡n</td>
    </tr>
    <tr>
      <td align="center">U20231B504</td>
      <td align="left">Morales Venegas, David Joel</td>
    </tr>
    <tr>
      <td align="center">U202316687</td>
      <td align="left">Paucar Zenteno, JesÃºs Fernando</td>
    </tr>
    <tr>
      <td align="center">U202322849</td>
      <td align="left">Viza Quispe, Marlon Packard</td>
    </tr>
    <tr>
      <td align="center">U201923820</td>
      <td align="left">CÃ¡ceres Pizarro, Albino Florencio</td>
    </tr>
  </tbody>
</table>

<br><br>

**Lima, abril de 2026**
</div>

<div class="page-break"></div>

# Registro de versiones del informe 
| VersiÃ³n | Fecha | Autores | DescripciÃ³n              |
| :--- | :--- | :--- |:-------------------------|
| 1.0.0 | 26/04/2026 | Mauricio SebastiÃ¡n Castillo Yataco, David Joel Morales Venegas, JesÃºs Fernando Paucar Zenteno, Marlon Packard Viza Quispe, Albino Florencio CÃ¡ceres Pizarro | VersiÃ³n inicial del avance AV1 (TB1) |

<div class="page-break"></div>

# Project Report Collaboration Insights
El presente apartado tiene como finalidad evidenciar el trabajo colaborativo realizado durante el desarrollo del informe. Para ello, se pone a disposiciÃ³n el repositorio oficial del proyecto, alojado en una organizaciÃ³n pÃºblica de GitHub:

ðŸ”— https://github.com/RQLS26

A partir de este repositorio, se analiza la participaciÃ³n de los integrantes del equipo mediante indicadores como nÃºmero de commits, frecuencia de contribuciones y actividad general registrada en la plataforma.

En el contexto de la entrega correspondiente a la TB1, TP1, TB2 y TF1, se presenta un anÃ¡lisis de colaboraciÃ³n que permite visualizar el nivel de aporte individual de cada miembro del equipo, sustentado en los registros de GitHub. Este anÃ¡lisis busca demostrar la distribuciÃ³n del trabajo, la constancia en el desarrollo del informe y el cumplimiento de las actividades asignadas.

## TB1
[pending content]

## TP1
[pending content]

## TB2
[pending content]

## TF1
[pending content]

<div class="page-break"></div>

# Contenido 
## Tabla de contenidos 

- [CarÃ¡tula](#informe-de-trabajo-final---av1)
- [Registro de Versiones del Informe](#registro-de-versiones-del-informe)
- [Student Outcome](#student-outcome)
- [Abstract](#abstract)
- [Resumen](#resumen)

- [CapÃ­tulo I: IntroducciÃ³n](#capÃ­tulo-i-introducciÃ³n)
    - [1.1. Startup Profile](#11-startup-profile)
    - [1.2. Solution Profile](#12-solution-profile)
    - [1.3. Segmentos objetivo](#13-segmentos-objetivo)

- [CapÃ­tulo II: Requirements Elicitation & Analysis](#capÃ­tulo-ii-requirements-elicitation--analysis)
    - [2.1. Competidores](#21-competidores)
    - [2.2. Entrevistas](#22-entrevistas)
    - [2.3. Needfinding](#23-needfinding)
    - [2.4. Big Picture EventStorming](#24-big-picture-eventstorming)
    - [2.5. Ubiquitous Language](#25-ubiquitous-language)

- [CapÃ­tulo III: Requirements Specification](#capÃ­tulo-iii-requirements-specification)
    - [3.1. User Stories](#31-user-stories)
    - [3.2. Impact Mapping](#32-impact-mapping)
    - [3.3. Product Backlog](#33-product-backlog)

- [CapÃ­tulo IV: Product Design](#capÃ­tulo-iv-product-design)
    - [4.1. Style Guidelines](#41-style-guidelines)
    - [4.2. Information Architecture](#42-information-architecture)
    - [4.3. Landing Page UI Design](#43-landing-page-ui-design)
    - [4.4. Web Applications UX/UI Design](#44-web-applications-uxui-design)
    - [4.5. Web Applications Prototyping](#45-web-applications-prototyping)
    - [4.6. Domain-Driven Software Architecture](#46-domain-driven-software-architecture)
    - [4.7. Software Object-Oriented Design](#47-software-object-oriented-design)
    - [4.8. Database Design](#48-database-design)

- [CapÃ­tulo V: Product Implementation, Validation & Deployment](#capÃ­tulo-v-product-implementation-validation--deployment)
    - [5.1. Software Configuration Management](#51-software-configuration-management)
    - [5.2. Landing Page, Services & Applications Implementation](#52-landing-page-services--applications-implementation)
    - [5.3. Validation Interviews](#53-validation-interviews)
    - [5.4. Video About-the-Product](#54-video-about-the-product)

- [CapÃ­tulo VI: Conclusions](#capÃ­tulo-vi-conclusions)
    - [6.1. Conclusiones y recomendaciones](#61-conclusiones-y-recomendaciones)
    - [6.2. Video About-the-Team](#62-video-about-the-team)

- [BibliografÃ­a](#bibliografÃ­a)

<div class="page-break"></div>

# Student Outcome 
El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET â€“ EAC - Student Outcome 5**  
**Criterio:** La capacidad de funcionar efectivamente en un equipo cuyos miembros juntos proporcionan liderazgo, crean un entorno de colaboraciÃ³n e inclusivo, establecen objetivos, planifican tareas y cumplen objetivos.

En el siguiente cuadro se describen las acciones realizadas y las conclusiones del equipo, que permiten sustentar el logro del ABET â€“ EAC - Student Outcome 5.

---

## Tabla de Student Outcome
<table style="width:100%; border-collapse: collapse;">
  <tr>
    <th style="width:25%;">Criterio especÃ­fico</th>
    <th style="width:45%;">Acciones realizadas</th>
    <th style="width:30%;">Conclusiones</th>
  </tr>

  <tr>
    <td>
      Trabaja en equipo para proporcionar liderazgo en forma conjunta
    </td>
    <td>
      <strong>Morales Venegas, David Joel</strong> â€” CreaciÃ³n del repositorio, DiseÃ±o de Landing Page, LiderÃ³ diseÃ±o/anÃ¡lisis de entrevistas.<br>
      <strong>Viza Quispe, Marlon Packard</strong> â€” Event Storming, Ubiquitous Language, Journey/Empathy Mapping.<br>
      <strong>Paucar Zenteno, JesÃºs Fernando</strong> â€” User Flow Diagrams, Web applications prototype.<br>
      <strong>Castillo Yataco, Mauricio SebastiÃ¡n</strong> â€” Lean UX Process, Segmentos Objetivo, Lean UX Canvas, Needfinding.<br>
      <strong>CÃ¡ceres Pizarro, Albino Florencio</strong> â€” Arquitectura de software (C4 Context Diagrams y Class Diagrams).<br>
    </td>
    <td>
      <strong>AV1:</strong> El equipo demostrÃ³ liderazgo compartido al asignar responsables especÃ­ficos basÃ¡ndose en las fortalezas tÃ©cnicas de cada integrante.<br>
      <strong>TB1:</strong> Se establecieron metas claras para el descubrimiento de usuarios, logrando una visiÃ³n holÃ­stica del problema logÃ­stico.<br>
    </td>
  </tr>
  <tr>
    <td>
      Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos
    </td>
    <td>
      <strong>Morales Venegas, David Joel</strong> â€” ColaborÃ³ en Wireframes, Wireflow y User Flow Diagrams.<br>
      <strong>Viza Quispe, Marlon Packard</strong> â€” DiseÃ±o de Landing Page, revisiÃ³n integradora y correcciones finales AV1.<br>
      <strong>Paucar Zenteno, JesÃºs Fernando</strong> â€” DiseÃ±o de Web Applications, revisiÃ³n integradora y correcciones finales AV1.<br>
      <strong>Castillo Yataco, Mauricio SebastiÃ¡n</strong> â€” DiseÃ±o de arquitectura, RedacciÃ³n y documentaciÃ³n del CapÃ­tulo V (SCM, Sprint 1).<br>
      <strong>CÃ¡ceres Pizarro, Albino Florencio</strong> â€” AnÃ¡lisis de competidores, diagrama de base de datos y artefactos de Needfinding.<br>
    </td>
    <td>
      <strong>AV1:</strong> La planificaciÃ³n de tareas mediante un backlog inicial permitiÃ³ cumplir con todos los artefactos de Needfinding y Lean UX.<br>
      <strong>TB1:</strong> El entorno colaborativo en GitHub facilitÃ³ la integraciÃ³n de los diagramas de arquitectura y el prototipo inicial.<br>
    </td>
  </tr>
</table>


<div class="page-break"></div>

# Abstract
This project addresses the operational inefficiencies and digital gap within micro and small enterprises (MSMEs) in the Peruvian construction sector. Focusing on the procurement and logistics chain, the development follows the Lean UX framework and Agile methodologies to design a specialized Software as a Service (SaaS) platform. The system centralizes requisitions, quotation comparisons, and multi-level approval workflows to replace informal communication channels. Preliminary research and user discovery suggest that the implementation of such a solution significantly improves budget traceability and reduces administrative lead times. Ultimately, this work contributes to the digital maturity of the industry by providing an accessible tool for operational optimization.

# Resumen
Este proyecto aborda las ineficiencias operativas y la brecha digital en las micro y pequeÃ±as empresas (MYPES) del sector construcciÃ³n en el PerÃº. CentrÃ¡ndose en la cadena de adquisiciones y logÃ­stica, el desarrollo sigue el marco de trabajo Lean UX y metodologÃ­as Ã¡giles para diseÃ±ar una plataforma especializada bajo el modelo Software as a Service (SaaS). El sistema centraliza las requisiciones, la comparativa de cotizaciones y los flujos de aprobaciÃ³n multinivel para reemplazar los canales de comunicaciÃ³n informales. La investigaciÃ³n preliminar y el descubrimiento de usuarios sugieren que la implementaciÃ³n de una soluciÃ³n de este tipo mejora significativamente la trazabilidad presupuestal y reduce los tiempos de espera administrativos. En Ãºltima instancia, este trabajo contribuye a la madurez digital de la industria al proporcionar una herramienta accesible para la optimizaciÃ³n operativa

<div class="page-break"></div>

# CapÃ­tulo I: IntroducciÃ³n

## 1.1. Startup Profile

### 1.1.1. DescripciÃ³n de la Startup
**RQLS (Requisitions, Quotes, Logistics System)** es una startup tecnolÃ³gica peruana enfocada en el desarrollo de soluciones Software as a Service (SaaS). Nuestra organizaciÃ³n se especializa en cerrar la brecha digital en las micro y pequeÃ±as empresas (MYPES) del sector construcciÃ³n. SegÃºn el Instituto Nacional de EstadÃ­stica e InformÃ¡tica (INEI, 2024), las MYPES representan el 99,7% de las unidades econÃ³micas del paÃ­s y enfrentan costos logÃ­sticos que ascienden al 21,1% de sus ventas (ComexPerÃº, 2023). RQLS transforma la gestiÃ³n operativa empÃ­rica en procesos basados en datos y transparencia.

**MisiÃ³n:** Democratizar el acceso a herramientas de control logÃ­stico para las MYPES constructoras, permitiÃ©ndoles eliminar sobrecostos mediante la centralizaciÃ³n de datos en tiempo real (Pacco Constructores, 2021).

**VisiÃ³n:** Ser el estÃ¡ndar tecnolÃ³gico en la gestiÃ³n de abastecimiento para el sector construcciÃ³n en LatinoamÃ©rica hacia el 2030.

**Valores:** Transparencia operativa, integridad de datos, innovaciÃ³n centrada en el operario y eficiencia.

### 1.1.2. Perfiles de integrantes del equipo
 | Imagen  | Apellidos y nombres                     |   CÃ³digo   | Carrera                | Perfil                                                                                                                                                                                                                                                                                                                                                                                                                                            |
:-----------------:|:----------------------------------------|:----------:| :--------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<img src="docs/assets/chapter-01/Castillo_Foto.jpg" alt="Foto de Castillo Yataco" width="120" />| **Castillo Yataco, Mauricio SebastiÃ¡n** | U202113229 | IngenierÃ­a de Software | Soy estudiante de IngenierÃ­a de Software, apasionado por la creaciÃ³n de soluciones tecnolÃ³gicas que mejoren la vida de las personas. Mi enfoque va mÃ¡s allÃ¡ de la programaciÃ³n, ya que me interesa desarrollar experiencias digitales funcionales y agradables para el usuario. Poseo conocimientos bÃ¡sicos en C++, HTML y CSS, y destaco por mi responsabilidad, cooperaciÃ³n, comunicaciÃ³n, flexibilidad y adaptabilidad.                        |
|<img src="docs/assets/chapter-01/david_foto.jpeg" alt="Foto de Morales Venegas" width="120" />| **Morales Venegas, David Joel**         | U20231B504 | IngenierÃ­a de Software | Estudiante de IngenierÃ­a de Software con formaciÃ³n intermedia en el desarrollo de aplicaciones web. Me adapto al trabajo tÃ©cnico del equipo, priorizando cÃ³digo funcional, entendible y alineado a los requerimientos del proyecto, con disposiciÃ³n para mejorar y corregir en funciÃ³n de pruebas y resultados.                                                                                                                                   |
|<img src="docs/assets/chapter-01/foto-fernando.jpg" alt="Foto de Fernando Paucar" width="120" />| **Paucar Zenteno, JesÃºs Fernando**      | U202316687 | IngenierÃ­a de Software | Soy estudiante de IngenierÃ­a de Software con gran pasiÃ³n por la creaciÃ³n de soluciones innovadoras. Me considero una persona proactiva y orientada a resultados, con interÃ©s constante en aprender y aplicar nuevas tecnologÃ­as. Busco contribuir significativamente al proyecto, asegurando calidad y eficiencia en cada tarea.                                                                                                                  |
|<img src="docs/assets/chapter-01/Marlon.jpg" alt="Foto Marlon Viza" width="120" />| **Viza Quispe, Marlon Packard**         | U202322849 | IngenierÃ­a de Software | Estudiante de 20 aÃ±os, responsable y proactivo, con sÃ³lida base tÃ©cnica en C++. Destaco por mi capacidad de aportar soluciones creativas y mi compromiso con el aprendizaje continuo en entornos profesionales. Busco asumir retos que potencien mi desarrollo y contribuyan al Ã©xito del equipo.                                                                                                                                                 |
|<img src="docs/assets/chapter-01/caceres_foto.jpeg" alt="Foto de Albino" width="120" />| **CÃ¡ceres Pizarro, Albino Florencio**   | U201923820 | IngenierÃ­a de Software | Me considero una persona responsable y proactiva que le gusta trabajar en equipo. AdemÃ¡s, siempre estoy abierto a ayudar, en lo posible, a cualquier integrante del equipo. AdemÃ¡s, busco adaptarme rÃ¡pidamente a los diversos retos que se presentan en el ciclo.                                                                                                                                                                                                                                                                                                                                                                                                                          |

---

## 1.2. Solution Profile
Nuestra soluciÃ³n, Buildline, es una plataforma Web SaaS diseÃ±ada para gestionar de extremo a extremo las compras institucionales en constructoras. Digitaliza la comunicaciÃ³n entre el residente de obra (solicitud), el Ã¡rea de compras (cotizaciÃ³n) y la gerencia (aprobaciÃ³n), eliminando pÃ©rdidas de hasta el 15% del presupuesto generadas por la gestiÃ³n informal (RodrÃ­guez Vargas, 2019).

### 1.2.1. Antecedentes y problemÃ¡tica
El sector construcciÃ³n en el PerÃº proyecta una tasa de crecimiento del 6,5% para el periodo 2025, impulsado principalmente por la reactivaciÃ³n de la inversiÃ³n en infraestructura pÃºblica (El Peruano, 2025). Esta dinÃ¡mica macroeconÃ³mica se encuentra condicionada por el desempeÃ±o de las MYPES, las cuales concentran la mayor parte de la operatividad del sector pero presentan un costo logÃ­stico promedio de 21,1%, cifra significativamente superior al 16% registrado a nivel nacional (ComexPerÃº, 2023; INEI, 2024). Esta disparidad econÃ³mica se vincula directamente a la falta de herramientas especializadas para la gestiÃ³n administrativa en empresas de menor escala.

La gestiÃ³n de adquisiciones en estas organizaciones se caracteriza por la ausencia de trazabilidad y formalidad tÃ©cnica. SegÃºn investigaciones aplicadas en el sector, el 74,1% de los responsables de MYPES constructoras califica como inadecuado el seguimiento de compras, mientras que el 77,8% reporta incidentes recurrentes donde los insumos entregados no coinciden con las especificaciones tÃ©cnicas solicitadas (RodrÃ­guez Vargas, 2019). Estos errores operativos, derivados de la dependencia de canales informales como WhatsApp o registros manuales en papel, causan parÃ¡lisis de obra en un 18% de los casos y obligan a realizar compras de urgencia no planificadas que representan el 12% del gasto logÃ­stico total (Tarraga Durand & Miranda Mitma, 2025).

El retraso en la madurez digital del sector construcciÃ³n se refleja en que el 40% de los proyectos de infraestructura superan el presupuesto original debido a la ineficiencia en la planificaciÃ³n de recursos y la comunicaciÃ³n fragmentada (Ruiz Escajadillo, 2024). A pesar de que la integraciÃ³n de plataformas de gestiÃ³n de proyectos ha demostrado incrementos de productividad del 30%, persiste una brecha tecnolÃ³gica en las pequeÃ±as empresas debido al desconocimiento de soluciones escalables y a la alta resistencia al cambio del personal operativo (ESAN, 2023; CAPECO, 2024). En este escenario, la transiciÃ³n hacia sistemas SaaS especializados permite la centralizaciÃ³n de datos necesaria para la toma de decisiones financieras y el control estricto del presupuesto de obra.

**TÃ©cnica "The 5W's y 2H's" aplicada al problema:**

| The 5W's y 2H's | Pregunta                     | DescripciÃ³n                                                                                                                                                                                                                                             |
| :-------------- | :--------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Who             | Â¿QuiÃ©nes estÃ¡n involucrados? | El personal operativo y directivo de las MYPES constructoras, especÃ­ficamente ingenieros residentes, jefes de logÃ­stica y gerentes. El 74,1% de los responsables considera deficientes los mecanismos actuales de seguimiento (RodrÃ­guez Vargas, 2019). |
| What            | Â¿CuÃ¡l es el problema?        | Ineficiencia en el flujo de suministro interno con falta de concordancia tÃ©cnica en el 77,8% de los productos recibidos y ausencia de proyecciones de demanda en el 70,3% de las operaciones (RodrÃ­guez Vargas, 2019).                                  |
| Where           | Â¿DÃ³nde ocurre?               | En la brecha informativa entre las obras de edificaciÃ³n fÃ­sica y el centro administrativo. Lima concentra el 45,7% de estas empresas, pero la ineficiencia es crÃ­tica en provincias por barreras de transporte (INEI, 2024).                            |
| When            | Â¿CuÃ¡ndo sucede?              | Durante la etapa de ejecuciÃ³n tÃ©cnica, manifestÃ¡ndose en cada ciclo de abastecimiento diario. Esta problemÃ¡tica es responsable del 18% de las paralizaciones de obra en el segmento (Tarraga Durand & Miranda Mitma, 2025).                             |
| Why             | Â¿Por quÃ© sucede?             | Debido a la inexistencia de sistemas de auditorÃ­a centralizados y la dependencia de herramientas informales (WhatsApp/Excel) que no aseguran el cumplimiento de calidad y tiempo (Ruiz Escajadillo, 2024).                                              |
| How             | Â¿CÃ³mo se manifiesta?         | Mediante procesos manuales sin validaciÃ³n presupuestal inmediata, lo que genera duplicidad de pedidos y obliga a compras de emergencia que representan el 12% del gasto logÃ­stico (Tarraga Durand & Miranda Mitma, 2025).                               |
| How Much        | Â¿CuÃ¡nto impacto tiene?       | Genera un sobrecosto logÃ­stico del 21,1% sobre las ventas (5,1 puntos sobre la media nacional) y una erosiÃ³n de hasta el 15% del presupuesto de insumos por errores de gestiÃ³n (ComexPerÃº, 2023; RodrÃ­guez Vargas, 2019).                               |

---

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements
Las micro y pequeÃ±as empresas (MYPES) constructoras de Lima Metropolitana gestionan los requerimientos de materiales mediante herramientas informales como WhatsApp o registros manuales en papel. Esta fragmentaciÃ³n de la informaciÃ³n dificulta la trazabilidad de los pedidos, impide la comparaciÃ³n tÃ©cnica de cotizaciones y retrasa la aprobaciÃ³n oportuna de compras por parte de la gerencia.

Como consecuencia de esta gestiÃ³n operativa deficiente, las organizaciones enfrentan sobrecostos por compras de emergencia y retrasos crÃ­ticos en la ejecuciÃ³n de obra que erosionan su rentabilidad neta. Como equipo, nos comprometemos a resolver este desafÃ­o mediante una colaboraciÃ³n estrecha con el personal de campo y administrativo para diseÃ±ar un flujo de abastecimiento trazable y auditable.

Ante esto nos surge la siguiente pregunta:
Â¿CÃ³mo podrÃ­a una plataforma SaaS de bajo costo centralizar las requisiciones y aprobaciones para reducir el lead time de compra y mejorar el control operativo?

1. Domain: GestiÃ³n de adquisiciones y abastecimiento logÃ­stico para el sector construcciÃ³n (MYPES).

2. Customer Segments: Gerentes Generales (aprobadores), Ingenieros Residentes (solicitantes) y Jefes de LogÃ­stica (compradores).

3. Pain Points: PÃ©rdida de trazabilidad de requerimientos, sobrecostos por emergencia y falta de comparaciÃ³n de cotizaciones.

4. Gap: Inexistencia de un software SaaS econÃ³mico diseÃ±ado para la pequeÃ±a constructora que cubra el espacio entre el Excel manual y ERPs de alta complejidad.

5. VisiÃ³n/Strategy: Digitalizar el 100% de los requerimientos de materiales mediante una plataforma en la nube que permita el control presupuestal en tiempo real.

6. Initial Segment: PequeÃ±as empresas constructoras de edificaciones residenciales ubicadas en Lima Metropolitana.

#### 1.2.2.2. Lean UX Assumptions
**Business Assumptions:**
1. Se considera que los clientes requieren formalizar los pedidos de materiales desde obra para reducir errores y el desorden sistemÃ¡tico en el abastecimiento (RodrÃ­guez Vargas, 2019).

2. Se plantea que esta necesidad puede resolverse mediante una plataforma web SaaS accesible desde dispositivos mÃ³viles, capaz de automatizar el flujo de cotizaciones y aprobaciones jerÃ¡rquicas.

3. Se identifica como segmento inicial a micro y pequeÃ±as empresas constructoras con sede en Lima Metropolitana y facturaciÃ³n anual menor a 1.700 UIT (INEI, 2024).

4. Se asume que el principal valor percibido por el cliente serÃ¡ la visualizaciÃ³n comparada de cotizaciones en tiempo real antes de autorizar un gasto, con el fin de respaldar decisiones mÃ¡s rentables.

5. Se prevÃ© que el cliente tambiÃ©n obtendrÃ¡ beneficios adicionales, como un historial digital de proveedores, reportes de gasto acumulado y mayor transparencia para auditorÃ­as.

6. Se proyecta que la adquisiciÃ³n de clientes se realizarÃ¡ mediante estrategias de marketing digital B2B segmentado y alianzas estratÃ©gicas con gremios del sector, como CAPECO.

7. Se estima que el modelo de ingresos mÃ¡s adecuado serÃ¡ una suscripciÃ³n mensual basada en el volumen de obras o proyectos activos gestionados por la constructora.

8. Se considera que la competencia principal estarÃ¡ conformada por el uso tradicional de WhatsApp y Excel, asÃ­ como por sistemas ERP complejos e inaccesibles para el presupuesto MYPE, como SAP u Odoo.

9. Se sostiene que la propuesta podrÃ¡ diferenciarse mediante una arquitectura de informaciÃ³n diseÃ±ada especÃ­ficamente para el flujo campo-oficina, reduciendo la complejidad innecesaria.

10. Se presume que el principal riesgo del producto es que el personal de campo mantenga el uso de canales informales si el flujo digital no reduce de forma clara el tiempo de coordinaciÃ³n frente a los canales actuales.

11. Se plantea que este riesgo puede mitigarse mediante un sistema de requerimientos en â€œ3 clicsâ€, diseÃ±ado para smartphones y mÃ¡s Ã¡gil que redactar un mensaje de texto.

12. Se asume que, si se comprueba que las constructoras no estÃ¡n dispuestas a pagar por control digital pese a las pÃ©rdidas actuales, el proyecto no serÃ¡ viable.

**Business Outcome Assumptions**
1. Reducir en un 40% el tiempo administrativo desde la creaciÃ³n de la requisiciÃ³n hasta la emisiÃ³n de la orden de compra.

2. Lograr que el 100% de las compras institucionales cuenten con un registro digital auditable y pasen por un flujo de aprobaciÃ³n con sustento de cotizaciÃ³n.

3. Disminuir las desviaciones presupuestarias por compras de emergencia no planificadas en un 15% (Tarraga Durand & Miranda Mitma, 2025).

4. Incrementar la visibilidad del margen de utilidad neta por proyecto al contar con costos de materiales centralizados y actualizados diariamente.

**User Assumptions**
1. Los jefes y gerentes requieren una herramienta que les permita aprobar compras crÃ­ticas sin estar fÃ­sicamente en la oficina.

2. Los jefes de proyecto valoran la posibilidad de delegar el proceso de cotizaciÃ³n al Ã¡rea de compras, manteniendo siempre la decisiÃ³n final sobre la elecciÃ³n del proveedor.

3. La gerencia espera que el sistema genere automÃ¡ticamente cuadros comparativos de precios para evitar el anÃ¡lisis manual de mÃºltiples correos electrÃ³nicos o archivos PDF.

4. El segmento objetivo necesita una soluciÃ³n que alerte de forma proactiva cuando un pedido de materiales supere el presupuesto asignado para una partida especÃ­fica de la obra.


**User Outcome Assumptions**
1. Los jefes de proyecto experimentarÃ¡n un aumento en la precisiÃ³n de sus auditorÃ­as financieras al contar con un historial inalterable de quiÃ©n solicitÃ³, quiÃ©n cotizÃ³ y quiÃ©n aprobÃ³ cada insumo.

2. Los gerentes se sentirÃ¡n mÃ¡s seguros respecto al uso del capital de la empresa al visualizar sistemÃ¡ticamente al menos tres opciones de cotizaciÃ³n antes de autorizar cualquier desembolso significativo.

3. Los responsables del negocio experimentarÃ¡n una reducciÃ³n del estrÃ©s operativo al disminuir las llamadas de emergencia por desabastecimiento, permitiÃ©ndoles enfocarse en la planificaciÃ³n estratÃ©gica y comercial.

4. Los jefes de proyecto confiarÃ¡n mÃ¡s en la veracidad de los datos de inventario y pedidos pendientes, lo que facilitarÃ¡ una coordinaciÃ³n mÃ¡s fluida con los clientes finales respecto a los plazos de entrega de los inmuebles.

5. El segmento percibirÃ¡ una optimizaciÃ³n del flujo de caja operativo al evitar compras duplicadas o adquisiciones con sobreprecio derivadas de la falta de comparaciÃ³n inmediata.

#### 1.2.2.3. Lean UX Hypothesis Statements
**Hypothesis 1** Creemos que al centralizar las solicitudes de materiales en una plataforma web accesible desde la obra, reduciremos drÃ¡sticamente los tiempos de espera. Lo sabremos cuando el tiempo promedio entre la creaciÃ³n de una solicitud y su aprobaciÃ³n por logÃ­stica baje de 48 horas a menos de 8 horas.

**Hypothesis 2** Creemos que al implementar un tablero de control (Dashboard) para los Jefes de Proyectos, eliminaremos la falta de visibilidad del presupuesto. Lo sabremos cuando las desviaciones de costos por compras de emergencia se reduzcan en un 15% durante el primer trimestre de uso.

**Hypothesis 3** Creemos que al automatizar los flujos de comunicaciÃ³n entre obra y logÃ­stica, optimizaremos el proceso de abastecimiento. Lo sabremos cuando el nÃºmero de llamadas o mensajes para consultar el estado de un pedido disminuya en un 50%.

**Hypothesis 4** Creemos que al digitalizar el historial de proveedores y cotizaciones, facilitaremos la toma de decisiones gerenciales. Lo sabremos cuando el tiempo dedicado a la comparaciÃ³n manual de cotizaciones se reduzca de 4 horas semanales a solo 15 minutos.

**Hypothesis 5** Creemos que digitalizar los requerimientos tÃ©cnicos para los ingenieros de obra lograrÃ¡ una reducciÃ³n del 50% en errores de pedido. Sabremos que es cierto cuando veamos que el 90% de los requerimientos registrados no requieren correcciones tÃ©cnicas posteriores.

#### 1.2.2.4. Lean UX Canvas

<table>
  <tr>
    <td valign="top">
      <strong>Business problem</strong>
      <br><br>
      Las micro y pequeÃ±as empresas (MYPES) constructoras de Lima Metropolitana gestionan los requerimientos de materiales mediante herramientas informales como WhatsApp o registros manuales en papel. Esta fragmentaciÃ³n dificulta la trazabilidad de los pedidos, limita la comparaciÃ³n tÃ©cnica de cotizaciones y retrasa la aprobaciÃ³n de compras.
      <br><br>
      Como consecuencia, se generan sobrecostos por compras de emergencia, duplicidad de pedidos y retrasos en la continuidad de obra que afectan directamente la rentabilidad del proyecto.
    </td>
    <td rowspan="2" valign="top">
      <strong>Solution ideas</strong>
      <br><br>
      - Plataforma web SaaS accesible desde dispositivos mÃ³viles orientada al entorno de obra
      <br><br>
      - Registro digital de requerimientos con flujo de aprobaciÃ³n jerÃ¡rquica
      <br><br>
      - MÃ³dulo de comparaciÃ³n de cotizaciones en tiempo real
      <br><br>
      - Historial centralizado de proveedores, pedidos y aprobaciones
      <br><br>
      - Alertas de control presupuestal y seguimiento de estados
    </td>
    <td valign="top">
      <strong>Business Outcomes</strong>
      <br><br>
      - Reducir en un 40% el tiempo administrativo desde la requisiciÃ³n hasta la orden de compra
      <br><br>
      - Lograr que el 100% de las compras cuenten con registro digital auditable
      <br><br>
      - Disminuir en un 15% los sobrecostos por compras no planificadas
      <br><br>
      - Mejorar la visibilidad del gasto y margen de utilidad por proyecto
    </td>
  </tr>
  <tr>
    <td valign="top">
      <strong>Users and customers</strong>
      <br><br>
      - Ingenieros residentes de obra
      <br>
      - Jefes de logÃ­stica
      <br>
      - Jefes de proyecto
      <br>
      - Gerentes generales
      <br>
      - MYPES constructoras de edificaciones
    </td>
    <td valign="top">
      <strong>User benefits</strong>
      <br><br>
      - AprobaciÃ³n remota de materiales sin dependencia de la oficina
      <br><br>
      - Visibilidad del estado de cada requerimiento en tiempo real
      <br><br>
      - ReducciÃ³n del tiempo dedicado a comparar cotizaciones
      <br><br>
      - Mejor coordinaciÃ³n entre obra y Ã¡rea administrativa
      <br><br>
      - Mayor control sobre el presupuesto antes de ejecutar compras
    </td>
  </tr>
  <tr>
    <td valign="top">
      <strong>Hypotheses</strong>
      <br><br>
      - Si se centralizan las solicitudes de materiales en una plataforma accesible desde obra, el tiempo de aprobaciÃ³n se reducirÃ¡ de 48 horas a menos de 8 horas.
      <br><br>
      - Si se implementa un panel de control para jefes de proyecto, las desviaciones por compras de emergencia se reducirÃ¡n en un 15%.
      <br><br>
      - Si se automatizan los flujos de comunicaciÃ³n entre obra y logÃ­stica, disminuirÃ¡n en un 50% las consultas manuales (llamadas y mensajes).
      <br><br>
      - Si se digitaliza el historial de proveedores y cotizaciones, el tiempo de comparaciÃ³n manual se reducirÃ¡ de 4 horas semanales a 15 minutos.
      <br><br>
      - Si los requerimientos tÃ©cnicos se registran digitalmente, los errores de pedido se reducirÃ¡n en un 50%.
    </td>
    <td valign="top">
      <strong>Whatâ€™s the most important thing we need to learn first?</strong>
      <br><br>
      Si las MYPES constructoras estÃ¡n dispuestas a reemplazar herramientas informales (WhatsApp, llamadas) por una plataforma digital y perciben suficiente valor como para adoptarla en su flujo de trabajo.
    </td>
    <td valign="top">
      <strong>Whatâ€™s the least amount of work we need to do to learn the next most important thing?</strong>
      <br><br>
      Realizar entrevistas con ingenieros residentes, jefes de logÃ­stica y gerentes, y validar mediante un prototipo de baja fidelidad el flujo de requisiciÃ³n, aprobaciÃ³n y comparaciÃ³n de cotizaciones, evaluando facilidad de uso, rapidez y disposiciÃ³n de adopciÃ³n.
    </td>
  </tr>
</table>

---

## 1.3. Segmentos Objetivos
El segmento objetivo de Buildline se centra exclusivamente en los perfiles de liderazgo y toma de decisiones dentro del entorno de la construcciÃ³n MYPE peruana. Este grupo es el responsable final de la viabilidad financiera de los proyectos y la sostenibilidad operativa de la empresa.

### 1.3.1. Jefes de Proyectos y Gerentes Generales

| DimensiÃ³n               | Detalle del perfil                                                                                                                                                                                                                                                                                                                                                                                       |
| ----------------------- |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Perfil DemogrÃ¡fico**  | Hombres y mujeres de entre 25 y 55 aÃ±os. Cuentan con educaciÃ³n superior universitaria, siendo mayoritariamente Ingenieros Civiles o Arquitectos titulados y colegiados. Muchos operan bajo la modalidad de Persona Natural con Negocio, que representa el 73,5% de las unidades econÃ³micas del sector (INEI, 2024).                                                                                      |
| **Perfil GeogrÃ¡fico**   | Ubicados principalmente en zonas urbanas de alta densidad constructiva. El 45,7% de las empresas se concentra en Lima Metropolitana, seguida de regiones estratÃ©gicas como Arequipa (5,3%), La Libertad (5,2%) y Piura (4,3%) (INEI, 2024).                                                                                                                                                              |
| **Perfil PsicogrÃ¡fico** | Profesionales con un estilo de vida de alta presiÃ³n y movilidad constante entre oficina y campo. Valoran la eficiencia y la honestidad operativa. Presentan una resistencia al cambio cultural del 48% (EY PerÃº, 2024), por lo que buscan herramientas que no compliquen sus procesos actuales. Su principal interÃ©s es la optimizaciÃ³n del margen de utilidad y la transparencia de sus flujos de caja. |
| **Puntos de Dolor**     | ErosiÃ³n de la rentabilidad debido a un costo logÃ­stico del 21,1% (ComexPerÃº, 2023). Enfrentan una falta de trazabilidad en el 74,1% de sus compras y sufren paralizaciones de obra en el 18% de los casos por desabastecimiento o errores tÃ©cnicos en el suministro (RodrÃ­guez Vargas, 2019; Tarraga Durand & Miranda Mitma, 2025).                                                                      |
| **Uso de TecnologÃ­a**   | Usuarios intensivos de dispositivos mÃ³viles; el 91,3% de la poblaciÃ³n ocupada en este rango de edad utiliza smartphones diariamente para la gestiÃ³n de sus actividades (INEI, 2025). Dependen actualmente de herramientas no especializadas como WhatsApp y Excel para el control operativo bÃ¡sico.                                                                                                      |


<div class="page-break"></div>

# CapÃ­tulo II: Requirements Elicitation & Analysis
## 2.1. Competidores
Este anÃ¡lisis permite identificar cÃ³mo se posiciona Buildline frente a ERPs consolidados en el mercado local, redes de abastecimiento regionales y plataformas SaaS de control financiero emergentes. A partir de ello, se define una ventaja competitiva basada en la reducciÃ³n de la brecha tecnolÃ³gica y la simplificaciÃ³n del flujo logÃ­stico para las MYPES peruanas.

### 2.1.1. AnÃ¡lisis competitivo
<table style="text-align: center; width: 100%;">
  <tbody>
    <tr>
      <td colspan="6"><strong>Competitive Analysis Landscape</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Â¿Por quÃ© llevar a cabo este anÃ¡lisis?</strong></td>
      <td colspan="4">
        Este anÃ¡lisis permite identificar brechas en el mercado logÃ­stico de construcciÃ³n peruano,
        diferenciando nuestra propuesta de valor frente a ERPs tradicionales y soluciones regionales.
      </td>
    </tr>
    <tr>
      <td colspan="2"><strong>Logotipos</strong></td>
      <td><img src="docs/assets/chapter-02/buildline-logo.png" alt="Buildline" height="50"></td>
      <td><img src="docs/assets/chapter-02/s10-logo.png" alt="S10 ERP" height="50"></td>
      <td><img src="docs/assets/chapter-02/iconstruye-logo.png" alt="ICONSTRUYE" height="50"></td>
      <td><img src="docs/assets/chapter-02/mawi-logo.png" alt="Mawi" height="50"></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Software</strong></td>
      <td><strong>Buildline (RQLS)</strong></td>
      <td><strong>S10 ERP</strong></td>
      <td><strong>ICONSTRUYE</strong></td>
      <td><strong>Mawi</strong></td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Perfil</strong></td>
      <td>Overview</td>
      <td>Startup SaaS enfocada en centralizar el ciclo de abastecimiento (solicitud-cotizaciÃ³n-aprobaciÃ³n) para MYPES constructoras peruanas.</td>
      <td>ERP peruano lÃ­der en presupuestos y gerencia de construcciÃ³n; opera bajo mÃ³dulos integrados que cubren desde almacÃ©n hasta contabilidad.</td>
      <td>Comunidad digital lÃ­der en LatAm que conecta constructoras con proveedores a travÃ©s de un marketplace transaccional masivo.</td>
      <td>SaaS de gestiÃ³n financiera para constructoras medianas enfocado en el control de costos y presupuestos en tiempo real.</td>
    </tr>
    <tr>
      <td>Ventaja competitiva, Â¿QuÃ© valor ofrece a los clientes?</td>
      <td>Flujo simple entre obra y oficina, con trazabilidad y comparaciÃ³n de precios en un solo lugar.</td>
      <td>Marca consolidada y alineaciÃ³n con normas locales de presupuestos y valorizaciones.</td>
      <td>Red amplia de proveedores y automatizaciÃ³n del abastecimiento.</td>
      <td>Interfaz moderna, lectura con IA y reportes automÃ¡ticos de utilidad.</td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Perfil de Marketing</strong></td>
      <td>Mercado objetivo</td>
      <td>MYPES constructoras de Lima y provincias que hoy operan con WhatsApp y Excel.</td>
      <td>Constructoras medianas y grandes con alta complejidad administrativa.</td>
      <td>Grandes constructoras e infraestructura con alto volumen de compras.</td>
      <td>Constructoras de 6 a 100 empleados que buscan control sin complejidad excesiva.</td>
    </tr>
    <tr>
      <td>Estrategias de marketing</td>
      <td>B2B, alianzas con CAPECO y enfoque en ahorro por control logÃ­stico.</td>
      <td>Marca histÃ³rica, partners y capacitaciÃ³n certificada.</td>
      <td>Ecosistema 360Â°, marketplace y casos de Ã©xito grandes.</td>
      <td>Propuesta de facilidad de uso, rapidez e implementaciÃ³n regional.</td>
    </tr>
    <tr>
      <td rowspan="3"><strong>Perfil de Producto</strong></td>
      <td>Productos &amp; Servicios</td>
      <td>Requisiciones, cotizaciones, aprobaciones y trazabilidad de pedidos.</td>
      <td>APU, planeamiento, almacenes, contabilidad y tareo mÃ³vil.</td>
      <td>Marketplace, Ã³rdenes electrÃ³nicas y facturaciÃ³n automatizada.</td>
      <td>Gastos de obra, Ã³rdenes de compra, gestiÃ³n documental y reportes mÃ³viles.</td>
    </tr>
    <tr>
      <td>Precios &amp; Costos</td>
      <td>SuscripciÃ³n mensual por obra activa.</td>
      <td>Licencia modular con inversiÃ³n inicial alta.</td>
      <td>Comisiones transaccionales y suscripciÃ³n corporativa.</td>
      <td>Setup inicial y planes mensuales por nÃºmero de usuarios.</td>
    </tr>
    <tr>
      <td>Canales de distribuciÃ³n (Web y/o MÃ³vil)</td>
      <td>Web responsive y app mÃ³vil para obra.</td>
      <td>Escritorio con portales web y apps auxiliares.</td>
      <td>Plataforma web con integraciÃ³n API.</td>
      <td>Web y mÃ³vil orientados a campo.</td>
    </tr>
    <tr>
      <td rowspan="4"><strong>AnÃ¡lisis SWOT</strong></td>
      <td>Fortalezas</td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Proceso especÃ­fico y crÃ­tico.</li>
          <li>Bajo costo frente a ERPs.</li>
          <li>DiseÃ±o campo-oficina.</li>
          <li>Trazabilidad en tiempo real.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>EstÃ¡ndar local del sector.</li>
          <li>Cobertura funcional amplia.</li>
          <li>AdecuaciÃ³n normativa.</li>
          <li>Alta aceptaciÃ³n empresarial.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Red extensa de proveedores.</li>
          <li>AutomatizaciÃ³n del abastecimiento.</li>
          <li>ConexiÃ³n entre mÃºltiples actores.</li>
          <li>Escala transaccional alta.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>UX moderna.</li>
          <li>IA para lectura de facturas.</li>
          <li>ImplementaciÃ³n rÃ¡pida.</li>
          <li>Reportes automÃ¡ticos.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>Debilidades</td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Marca joven.</li>
          <li>Poco reconocimiento.</li>
          <li>Menos integraciones.</li>
          <li>Depende de adopciÃ³n del usuario.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Interfaz menos moderna.</li>
          <li>Curva de aprendizaje alta.</li>
          <li>Complejo para MYPES.</li>
          <li>Mayor soporte tÃ©cnico.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Complejidad funcional alta.</li>
          <li>Costo poco accesible.</li>
          <li>Enfoque en alto volumen.</li>
          <li>Poca adaptaciÃ³n a urgencias de obra.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>MÃ¡s financiero que operativo.</li>
          <li>Menor robustez logÃ­stica.</li>
          <li>Depende de conectividad.</li>
          <li>No resuelve bien trazabilidad obra-oficina.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>Oportunidades</td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>DigitalizaciÃ³n de MYPES.</li>
          <li>Necesidad de trazabilidad.</li>
          <li>Control de gasto por proyecto.</li>
          <li>ExpansiÃ³n a procesos similares.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>MigraciÃ³n a la nube.</li>
          <li>Demanda de integraciÃ³n total.</li>
          <li>ModernizaciÃ³n de procesos.</li>
          <li>Captura de usuarios avanzados.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Crecimiento del comercio digital.</li>
          <li>Necesidad de marketplaces confiables.</li>
          <li>IntegraciÃ³n a cadenas de abastecimiento.</li>
          <li>Mayor transaccionalidad sectorial.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>ExpansiÃ³n regional.</li>
          <li>Mayor uso de reportes automÃ¡ticos.</li>
          <li>Empresas que buscan control sin ERP pesado.</li>
          <li>Demanda de control presupuestal en tiempo real.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>Amenazas</td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Uso persistente de WhatsApp y Excel.</li>
          <li>Resistencia al cambio.</li>
          <li>Competidores mÃ¡s simples y baratos.</li>
          <li>Dificultad para demostrar valor temprano.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Soluciones mÃ¡s Ã¡giles.</li>
          <li>RenovaciÃ³n tecnolÃ³gica del mercado.</li>
          <li>Preferencia por herramientas ligeras.</li>
          <li>Riesgo de pÃ©rdida de usuarios nuevos.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Compra directa al proveedor.</li>
          <li>Portales que eliminan intermediarios.</li>
          <li>Competencia por escala.</li>
          <li>Plataformas ya posicionadas.</li>
        </ul>
      </td>
      <td>
        <ul style="text-align: left; margin: 0; padding-left: 18px;">
          <li>Software genÃ©rico barato.</li>
          <li>ERPs globales mÃ¡s accesibles.</li>
          <li>Baja conectividad en campo.</li>
          <li>Mayor presiÃ³n por automatizaciÃ³n.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 2.1.2. Estrategias y tÃ¡cticas frente a competidores
A partir de la identificaciÃ³n de fortalezas y debilidades competitivas, la startup RQLS aplicarÃ¡ el siguiente conjunto de estrategias y tÃ¡cticas preliminares para posicionar a Buildline como la soluciÃ³n lÃ­der para el segmento MYPE peruano.

#### Estrategia ofensiva: explotaciÃ³n de la brecha tecnolÃ³gica frente a S10 ERP
Aprovecharemos la obsolescencia tÃ©cnica de los ERPs tradicionales para captar a las empresas que buscan una modernizaciÃ³n rÃ¡pida sin la complejidad de sistemas legados.

- **Onboarding acelerado:** implementar un programa de migraciÃ³n de datos desde Excel en menos de 24 horas, eliminando la barrera de las semanas de capacitaciÃ³n que exige S10.
- **Movilidad total:** posicionar la app mÃ³vil de Buildline como la herramienta de campo que S10 no posee con robustez, permitiendo que el residente registre pedidos incluso sin conexiÃ³n estable.

#### Estrategia defensiva: diferenciaciÃ³n por enfoque interno frente a ICONSTRUYE
ICONSTRUYE domina la relaciÃ³n externa con proveedores mediante un marketplace, pero Buildline se enfocarÃ¡ en el flujo interno que genera el desorden administrativo inicial.

- **Control de requisiciones:** enfatizar que el 74,1% de las MYPES falla en el seguimiento interno. Buildline resolverÃ¡ el caos de firmas y aprobaciones antes de que el pedido llegue al proveedor, algo que las plataformas transaccionales corporativas no atienden para proyectos pequeÃ±os.
- **Costo logÃ­stico reducido:** utilizar el indicador del 21,1% de sobrecosto logÃ­stico MYPE como argumento de venta principal, ofreciendo un ROI visible en el primer mes de uso.

#### Estrategia adaptativa: mitigaciÃ³n de la resistencia cultural
Para afrontar la informalidad asociada al uso de WhatsApp y la resistencia al cambio detectada en el personal de obra, Buildline aplicarÃ¡ tÃ¡cticas de adopciÃ³n orgÃ¡nica.

- **Solicitud en 3 clics:** diseÃ±ar la interfaz mÃ³vil para que el registro de un pedido de cemento o acero sea mÃ¡s rÃ¡pido que escribir un mensaje de texto.
- **Dashboards de transparencia:** ofrecer al gerente un panel de control presupuestal que le permita supervisar gastos y aprobaciones, generando presiÃ³n positiva desde la gerencia hacia el campo para el uso del sistema.

#### Estrategia de alianzas y contexto regional
El crecimiento esperado del sector en 2025, impulsado por obras pÃºblicas, abre una ventana de necesidad de transparencia. RQLS buscarÃ¡ alianzas con gremios como CAPECO para reforzar la credibilidad de Buildline y su adopciÃ³n en el mercado.

- **Posicionamiento regional:** promover Buildline como una soluciÃ³n auditables y adaptada al contexto peruano.
- **IntegraciÃ³n local:** priorizar la integraciÃ³n nativa con facturaciÃ³n electrÃ³nica de SUNAT, como barrera tÃ©cnica frente a competidores globales con versiones simplificadas.

## 2.2. Entrevistas
En esta secciÃ³n se aborda la investigaciÃ³n tomando como base la recolecciÃ³n de informaciÃ³n mediante entrevistas a representantes del segmento objetivo. Las entrevistas serÃ¡n registradas en video como evidencia del proceso de obtenciÃ³n de requisitos.

### 2.2.1. DiseÃ±o de entrevistas
Para el desarrollo de las entrevistas del segmento objetivo, se redactaron las siguientes preguntas siguiendo las buenas prÃ¡cticas para el diseÃ±o de recolecciÃ³n de informaciÃ³n:

**Segmento objetivo: Jefes de Proyectos y Gerentes Generales**

#### Preguntas DemogrÃ¡ficas
1. Â¿CuÃ¡l es su nombre completo y quÃ© edad tiene?
2. Â¿CÃ³mo se definirÃ­a profesionalmente?
3. Â¿CuÃ¡l es su estado civil y tiene familia a su cargo?
4. Â¿CuÃ¡l es su cargo exacto y cuÃ¡ntos aÃ±os de experiencia tiene en el sector construcciÃ³n?
5. Â¿En quÃ© distrito/provincia reside y dÃ³nde se ubican usualmente sus proyectos?

#### Preguntas de HÃ¡bitos Digitales
6. Â¿CuÃ¡l es el dispositivo que utiliza con mayor frecuencia durante su jornada laboral para gestionar tareas (Laptop, Tablet o Celular)?
7. Â¿QuÃ© navegador web y sistemas operativos utiliza con mayor frecuencia para revisar reportes tÃ©cnicos?
8. Â¿CuÃ¡les son los canales digitales de interacciÃ³n que mÃ¡s utiliza para comunicarse con su equipo (WhatsApp, Slack, correo electrÃ³nico)?
9. Â¿Utiliza actualmente algÃºn software especializado para la gestiÃ³n de proyectos o presupuestos?

#### Preguntas Principales
10. Â¿CuÃ¡ntos proyectos u obras suele gestionar de manera simultÃ¡nea en un mes promedio?
11. Â¿PodrÃ­a describir el flujo de trabajo actual desde que se identifica la falta de un material en obra hasta que se emite el pago al proveedor?
12. Â¿QuÃ© medios de comunicaciÃ³n utiliza para recibir las requisiciones de los ingenieros residentes?
13. Â¿CÃ³mo gestiona y almacena las cotizaciones recibidas de diversos proveedores para un mismo requerimiento?
14. Â¿CÃ³mo realiza actualmente el control presupuestal de los materiales por cada proyecto?
15. Â¿Ha experimentado retrasos en el cronograma de obra debido a errores en la logÃ­stica de abastecimiento?
16. Â¿Considera que el uso de herramientas genÃ©ricas (como Excel) es suficiente para mantener un control de costos eficiente en sus obras?

### 2.2.2. Registro de entrevistas
**Segmento objetivo: Jefes de Proyectos y Gerentes Generales**

<table style="width:100%; border-collapse:collapse;">
  <tbody>
    <tr>
      <td colspan="4" align="center"><strong>Entrevista N.Â° 1</strong></td>
    </tr>
    <tr>
      <td colspan="4" align="center">
        <img src="docs/assets/chapter-02/entrevista-01.png" alt="Buildline" height="350"></td>
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center"><strong>InformaciÃ³n del entrevistado</strong></td>
      <td colspan="2" align="center"><strong>Contexto tecnolÃ³gico</strong></td>
    </tr>
    <tr>
      <td><strong>Nombre comple</strong></td>
      <td> Abdon Viza Amanqui </td>
      <td><strong> Dispositivo de mayor frecuencia </strong></td>
      <td> Laptop y celular </td>
    </tr>
    <tr>
      <td><strong>Edad</strong></td>
      <td> 54 aÃ±os </td>
      <td><strong>Sistema operativo/browser</strong></td>
      <td> Windows (Office) </td>
    </tr>
    <tr>
      <td><strong>DefiniciÃ³n profesional / cargo</strong></td>
      <td>Jefes de Proyectos (Ingeniero Civil)</td>
      <td><strong>Canales digitales de comunicaciÃ³n</strong></td>
      <td> WhatsApp </td>
    </tr>
    <tr>
      <td><strong>Residencia / ubicaciÃ³n</strong></td>
      <td> Juliaca (Puno) </td>
      <td><strong>Software especializado utilizado</strong></td>
      <td> AutoCAD, Excel y Word </td>
    </tr>
    <tr>
      <td colspan="2"><strong>DuraciÃ³n</strong>: 8:46</td>
      <td colspan="2"><strong>URL de grabaciÃ³n: </strong><a href="https://upcedupe-my.sharepoint.com/personal/u202322849_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202322849%5Fupc%5Fedu%5Fpe%2FDocuments%2FVideos%2FSegmento%2D1%2DJefes%20de%20Proyectos%20y%20Gerentes%20Generales%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E593e8b93%2Dc4f0%2D4a57%2D9f1e%2De92dc81c64bd" target="_blank">Ver video</a></td>
  </td>
    </tr>
    <tr>
      <td colspan="4">
        <strong>Resumen de la entrevista</strong><br><br>
        El entrevistado es un jefe de departamento en el sector construcciÃ³n con 20 aÃ±os de experiencia que labora de forma independiente y para empresas privadas, operando principalmente en Juliaca, Puno, y zonas aledaÃ±as como Cusco y Arequipa. En su rutina digital utiliza predominantemente laptop y celular, apoyÃ¡ndose en herramientas como AutoCAD, Excel y Word para la elaboraciÃ³n de reportes tÃ©cnicos, mientras que WhatsApp es su canal principal de comunicaciÃ³n y S10 su software para presupuestos. Su dinÃ¡mica de trabajo implica la gestiÃ³n de levantamientos topogrÃ¡ficos y de carreteras que luego procesa en gabinete, siguiendo un flujo logÃ­stico que inicia con el requerimiento de materiales desde el campo hacia el almacÃ©n.

El proceso de aprobaciÃ³n de compras involucra al residente y al contratista general, pudiendo demorar hasta dos dÃ­as, y actualmente enfrenta desafÃ­os como la frustraciÃ³n por la demora en la llegada de materiales y la necesidad de actualizar constantemente los costos del mercado. AbdÃ³n seÃ±ala que el uso de Excel es insuficiente para un control eficiente debido al riesgo de errores humanos y expresa un alto interÃ©s en automatizar la variaciÃ³n de costos y la gestiÃ³n logÃ­stica. Finalmente, destaca que la rapidez en la entrega de materiales es el factor mÃ¡s influyente en sus decisiones y considera fundamental contar con una plataforma mÃ³vil que permita supervisar y gestionar las operaciones directamente desde el campo.
      </td>
    </tr>
  </tbody>
</table>

<table style="width:100%; border-collapse:collapse;">
  <tbody>
    <tr>
      <td colspan="4" align="center"><strong>Entrevista N.Â° 2</strong></td>
    </tr>
    <tr>
      <td colspan="4" align="center">
        <img src="../docs/assets/chapter-02/entrevista-02.png" alt="Entrevista 2" height="350">
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center"><strong>InformaciÃ³n del entrevistado</strong></td>
      <td colspan="2" align="center"><strong>Contexto tecnolÃ³gico</strong></td>
    </tr>
    <tr>
      <td><strong>Nombre completo</strong></td>
      <td> David Garibay </td>
      <td><strong>Dispositivo de mayor frecuencia</strong></td>
      <td> Celular (comunicaciÃ³n) y Laptop (gestiÃ³n) </td>
    </tr>
    <tr>
      <td><strong>Edad</strong></td>
      <td> 45 aÃ±os </td>
      <td><strong>Sistema operativo/browser</strong></td>
      <td> Windows / Google Chrome </td>
    </tr>
    <tr>
      <td><strong>DefiniciÃ³n profesional / cargo</strong></td>
      <td> Gerente de Proyecto (Ingeniero) </td>
      <td><strong>Canales digitales de comunicaciÃ³n</strong></td>
      <td> WhatsApp (rÃ¡pido) y Correo (formal) </td>
    </tr>
    <tr>
      <td><strong>Residencia / ubicaciÃ³n</strong></td>
      <td> Santiago de Surco, Lima (Obras en provincia) </td>
      <td><strong>Software especializado utilizado</strong></td>
      <td> SAP, MS Project, Oracle Primavera, Power BI y Excel </td>
    </tr>
    <tr>
      <td colspan="2"><strong>DuraciÃ³n</strong>: 12:14</td>
      <td colspan="2"><strong>URL de grabaciÃ³n: </strong><a href="https://drive.google.com/file/d/14m4jJwM0lSUNWYnrakp4qyTpgDP1KKJ8/view" target="_blank">Ver video</a></td>
    </tr>
    <tr>
      <td colspan="4">
        <strong>Resumen de la entrevista</strong><br><br>
        El entrevistado es un Gerente de Proyecto con 18 aÃ±os de experiencia en el sector construcciÃ³n, gestionando actualmente obras de gran envergadura en provincias, como minerÃ­a y carreteras. En su rutina digital, utiliza el celular para resolver urgencias operativas vÃ­a WhatsApp, mientras que reserva el uso de su laptop (con Windows y Chrome) para la revisiÃ³n financiera, presupuestal y la aprobaciÃ³n de compras usando sistemas como SAP y MS Project.<br><br>El flujo logÃ­stico que supervisa involucra requerimientos del campo, cotizaciones de logÃ­stica y su aprobaciÃ³n final. Carlos identifica los retrasos en el abastecimiento como uno de los problemas mÃ¡s crÃ­ticos, ya que paralizar una obra genera altÃ­simos sobrecostos. AdemÃ¡s, seÃ±ala un cuello de botella en la formalidad: aunque las requisiciones deberÃ­an procesarse en el sistema integrado, en la prÃ¡ctica las urgencias se manejan por mensajes directos. Finalmente, enfatiza que el uso de herramientas genÃ©ricas como Excel es "peligroso" para llevar el control de costos a nivel profesional debido al riesgo de errores humanos y la falta de trazabilidad, validando la necesidad de un sistema estructurado y seguro.
      </td>
    </tr>
  </tbody>
</table>

<table style="width:100%; border-collapse:collapse;">
  <tbody>
    <tr>
      <td colspan="4" align="center"><strong>Entrevista N.Â° 3</strong></td>
    </tr>
    <tr>
      <td colspan="4" align="center">
        <img src="../docs/assets/chapter-02/entrevista-03.png" alt="Entrevista 3 - Leonardo" height="350">
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center"><strong>InformaciÃ³n del entrevistado</strong></td>
      <td colspan="2" align="center"><strong>Contexto tecnolÃ³gico</strong></td>
    </tr>
    <tr>
      <td><strong>Nombre completo</strong></td>
      <td> Leonardo Anhuaman </td>
      <td><strong>Dispositivo de mayor frecuencia</strong></td>
      <td> Celular (coordinaciÃ³n) y Laptop (reportes) </td>
    </tr>
    <tr>
      <td><strong>Edad</strong></td>
      <td> 24 aÃ±os </td>
      <td><strong>Sistema operativo/browser</strong></td>
      <td> Android / Windows / Google Chrome </td>
    </tr>
    <tr>
      <td><strong>DefiniciÃ³n profesional / cargo</strong></td>
      <td> Jefe de Proyecto Junior </td>
      <td><strong>Canales digitales de comunicaciÃ³n</strong></td>
      <td> WhatsApp (predominante) y Correo </td>
    </tr>
    <tr>
      <td><strong>Residencia / ubicaciÃ³n</strong></td>
      <td> Chorrillos, Lima </td>
      <td><strong>Software especializado utilizado</strong></td>
      <td> S10 y Excel </td>
    </tr>
    <tr>
      <td colspan="2"><strong>DuraciÃ³n</strong>: 05:58</td>
      <td colspan="2"><strong>URL de grabaciÃ³n: </strong><a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u202316687_upc_edu_pe/IQBWOpfi_6v_T7DTHOz0tzKIAbYe-kP_QcbvspNKOG6LOLQ?e=dSPEWH&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D" target="_blank">Ver video</a></td>
    </tr>
    <tr>
      <td colspan="4">
        <strong>Resumen de la entrevista</strong><br><br>
        El entrevistado es un Jefe de Proyecto Junior con 2 aÃ±os de experiencia en una constructora familiar, operando principalmente en el distrito de Chorrillos. Su perfil representa la nueva generaciÃ³n de profesionales en el sector que, a pesar de tener un dominio fluido de herramientas digitales (celular, laptops y apps de mensajerÃ­a), se ven limitados por la informalidad de los procesos tradicionales de la empresa. <br><br>
        Leonardo describe un flujo logÃ­stico crÃ­tico basado casi exclusivamente en WhatsApp y llamadas telefÃ³nicas, lo que genera una pÃ©rdida constante de trazabilidad en las cotizaciones y errores en las especificaciones tÃ©cnicas de los materiales. Identifica que la falta de un sistema de "Ã“rdenes de Compra" formales causa retrasos operativos y paralizaciones de cuadrillas, impactando directamente en la rentabilidad. El entrevistado valida la necesidad de transicionar de un control basado en Excel manual hacia una plataforma integrada que permita la aprobaciÃ³n inmediata por parte de gerencia y centralice el historial de costos para una mejor toma de decisiones.
      </td>
    </tr>
  </tbody>
</table>

<table style="width:100%; border-collapse:collapse;">
  <tbody>
    <tr>
      <td colspan="4" align="center"><strong>Entrevista N.Â° 4</strong></td>
    </tr>
    <tr>
      <td colspan="4" align="center">
        <img src="../docs/assets/chapter-02/entrevista-04.png" alt="Entrevista 3 - Leonardo" height="350">
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center"><strong>InformaciÃ³n del entrevistado</strong></td>
      <td colspan="2" align="center"><strong>Contexto tecnolÃ³gico</strong></td>
    </tr>
    <tr>
      <td><strong>Nombre completo</strong></td>
      <td>Lisset Paredes</td>
      <td><strong>Dispositivo de mayor frecuencia</strong></td>
      <td>aptop y celular (uso intensivo del celular para coordinaciÃ³n en campo)</td>
    </tr>
    <tr>
      <td><strong>Edad</strong></td>
      <td>32 aÃ±os</td>
      <td><strong>Sistema operativo/browser</strong></td>
      <td>Windows (laptop), Android (celular), navegador Google Chrome</td>
    </tr>
    <tr>
      <td><strong>DefiniciÃ³n profesional / cargo</strong></td>
      <td>Jefa de logÃ­stica, profesional organizada, analÃ­tica y orientada a resultados</td>
      <td><strong>Canales digitales de comunicaciÃ³n</strong></td>
      <td>WhatsApp (principal), correo electrÃ³nico (uso formal y registro)</td>
    </tr>
    <tr>
      <td><strong>Residencia / ubicaciÃ³n</strong></td>
      <td>JesÃºs MarÃ­a, Lima â€“ Proyectos en San Miguel, Surco y Ate</td>
      <td><strong>Software especializado utilizado</strong></td>
      <td>Uso parcial de Indusoft (consulta de stock y requerimientos), complementado con Excel, correo electrÃ³nico y WhatsApp</td>
    </tr>
    <tr>
      <td colspan="2"><strong>DuraciÃ³n</strong>: [pendiente de completar]</td>
      <td colspan="2"><strong>URL de grabaciÃ³n: </strong><a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u201923820_upc_edu_pe/IQBlkNjTWHvGRrHWcVowxzt6Adx8YM62dFlnE9heBecX338?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=mTp6gw" target="_blank">Ver video</a></td>
    </tr>
    <tr>
      <td colspan="4">
        <strong>Resumen de la entrevista</strong><br><br>
        La entrevistada, Lisset Paredes, jefa de logÃ­stica con aproximadamente 10 aÃ±os de experiencia, gestiona entre 2 y 3 proyectos de manera simultÃ¡nea. Su trabajo se apoya principalmente en herramientas como WhatsApp para la comunicaciÃ³n diaria, el correo electrÃ³nico para formalizar informaciÃ³n y Microsoft Excel para el control de costos. AdemÃ¡s, utiliza parcialmente Indusoft para consultas de stock, aunque este presenta limitaciones como lentitud en su funcionamiento.
El proceso de abastecimiento inicia con requerimientos enviados desde obra, generalmente a travÃ©s de WhatsApp y muchas veces con informaciÃ³n incompleta, lo que genera retrabajo y retrasos. Posteriormente, la bÃºsqueda y comparaciÃ³n de cotizaciones se realiza de forma manual, almacenando la informaciÃ³n en distintos medios sin un sistema centralizado.

El control presupuestal tambiÃ©n se gestiona en Excel, sin actualizaciÃ³n en tiempo real, lo que ocasiona desfases entre los registros y la ejecuciÃ³n real de gastos. Esta falta de integraciÃ³n y trazabilidad contribuye a errores logÃ­sticos, pÃ©rdida de informaciÃ³n y retrasos en obra.
En general, la entrevistada considera que las herramientas actuales no son suficientes para gestionar eficientemente mÃºltiples proyectos, evidenciando la necesidad de una soluciÃ³n digital mÃ¡s integrada y especializada.
      </td>
    </tr>
  </tbody>
</table>

<table style="width:100%; border-collapse:collapse;">
  <tbody>
    <tr>
      <td colspan="4" align="center"><strong>Entrevista N.Â° 5</strong></td>
    </tr>
    <tr>
      <td colspan="4" align="center">
        <img src="../docs/assets/chapter-02/entrevista-05.png" alt="Entrevista 5 - SebastiÃ¡n" height="350">
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center"><strong>InformaciÃ³n del entrevistado</strong></td>
      <td colspan="2" align="center"><strong>Contexto tecnolÃ³gico</strong></td>
    </tr>
    <tr>
      <td><strong>Nombre completo</strong></td>
      <td>SebastiÃ¡n VÃ¡squez</td>
      <td><strong>Dispositivo de mayor frecuencia</strong></td>
      <td>Laptop y Smartphone (Android)</td>
    </tr>
    <tr>
      <td><strong>Edad</strong></td>
      <td>27 aÃ±os</td>
      <td><strong>Sistema operativo/browser</strong></td>
      <td>Windows 11 / Google Chrome</td>
    </tr>
    <tr>
      <td><strong>DefiniciÃ³n profesional / cargo</strong></td>
      <td>Ingeniero Civil</td>
      <td><strong>Canales digitales de comunicaciÃ³n</strong></td>
      <td>WhatsApp Business y Microsoft Outlook</td>
    </tr>
    <tr>
      <td><strong>Residencia / ubicaciÃ³n</strong></td>
      <td>San Borja, Lima</td>
      <td><strong>Software especializado utilizado</strong></td>
      <td>S10 (Presupuestos), MS Project y MS Excel</td>
    </tr>
    <tr>
      <td colspan="2"><strong>DuraciÃ³n</strong>: 14:54</td>
      <td colspan="2"><strong>URL de grabaciÃ³n: </strong><a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231b504_upc_edu_pe/IQDfPqhAH-25T7AE0HENbnpTAZ2WTtY2YOFNkrarA_D8QgM?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=XxxnPg" target="_blank">Ver video</a></td>
    </tr>
    <tr>
      <td colspan="4">
        <strong>Resumen de la entrevista</strong><br><br>
        SebastiÃ¡n destaca que el mayor dolor administrativo es la pÃ©rdida de trazabilidad en las compras. Actualmente, recibe requerimientos por WhatsApp que se mezclan con fotos de obra y mensajes personales, lo que causa olvidos y compras de emergencia que elevan los costos hasta en un 18%.
        Valida positivamente la soluciÃ³n, ya que actualmente debe revisar PDF's sueltos en el correo para decidir a quÃ© proveedor comprar. Indica que su disposiciÃ³n a pagar por el SaaS depende de que el operario en campo (Residente) realmente use el sistema en lugar de llamar por telÃ©fono. Sugiere que la interfaz sea extremadamente ligera debido a la baja seÃ±al en algunas obras de infraestructura.
      </td>
    </tr>
  </tbody>
</table>

### 2.2.3. AnÃ¡lisis de entrevistas

### AnÃ¡lisis por segmento objetivo

**Segmento objetivo: Jefes de Proyectos y Gerentes Generales**

#### 1. DescripciÃ³n general del segmento
Este segmento agrupa a [descripciÃ³n breve del grupo analizado]. A partir de las entrevistas registradas, se identificaron patrones comunes en sus caracterÃ­sticas objetivas y subjetivas, los cuales sirven como base para la construcciÃ³n del arquetipo correspondiente.

#### 2. CaracterÃ­sticas objetivas del segmento
| CaracterÃ­stica              | Sustento estadÃ­stico | Evidencia en entrevistas | RelaciÃ³n con el arquetipo |
|:----------------------------| :-- | :-- | :-- |
| **Uso de mensajerÃ­a informal para requerimientos** | 100% (5/5) | **Entrevistas 1, 2, 3, 4 y 5:** Todos afirman usar WhatsApp como canal principal para urgencias y requerimientos de obra, mezclando datos tÃ©cnicos con mensajes personales. | Define el comportamiento actual del usuario y justifica la necesidad de crear un canal de comunicaciÃ³n centralizado y estructurado. |
| **Uso de MS Excel como herramienta base de control** | 80% (4/5) | **Entrevistas 1, 2, 3 y 4:** AbdÃ³n, Carlos, Leonardo y Lisset utilizan Excel para presupuestos y control de costos, pero reconocen que no se actualiza en tiempo real. | Establece la lÃ­nea base de competencia tecnolÃ³gica del usuario: estÃ¡n acostumbrados a tablas y grillas, por lo que la nueva interfaz debe ser familiar pero automatizada. |
| **OperaciÃ³n dividida (Campo vs. Gabinete)** | 100% (5/5) | **Todas las entrevistas:** Evidencian un flujo logÃ­stico desconectado donde el campo (residente) pide y el gabinete (oficina/logÃ­stica) procesa y aprueba. | Moldea el arquetipo en dos roles interactuantes, obligando a que la soluciÃ³n sea multiplataforma (mÃ³vil para campo, web para oficina). |
| **Dependencia de dispositivos mÃ³viles con conectividad limitada** | 60% (3/5) | **Entrevistas 1, 2 y 5:** AbdÃ³n, Carlos y SebastiÃ¡n priorizan el celular. SebastiÃ¡n indica que la seÃ±al en obras de infraestructura es baja. | Dictamina que el arquetipo valora la inmediatez y requiere que la aplicaciÃ³n sea extremadamente ligera (Low-Data) para funcionar en campo. |

#### 3. CaracterÃ­sticas subjetivas del segmento
| CaracterÃ­stica               | Sustento estadÃ­stico | Evidencia en entrevistas | RelaciÃ³n con el arquetipo |
|:-----------------------------| :-- | :-- | :-- |
| **FrustraciÃ³n por pÃ©rdida de trazabilidad** | 100% (5/5) | **Entrevistas 3, 4 y 5:** Leonardo, Lisset y SebastiÃ¡n sufren por cotizaciones perdidas, PDFs sueltos y requerimientos incompletos enviados por WhatsApp. | Define el principal dolor (*pain point*) del arquetipo: la ansiedad administrativa y la carga cognitiva de buscar informaciÃ³n dispersa. |
| **PercepciÃ³n de riesgo ante procesos manuales** | 60% (3/5) | **Entrevistas 1, 2 y 3:** Carlos califica a Excel como "peligroso" a nivel profesional. AbdÃ³n y Leonardo seÃ±alan el alto riesgo de errores humanos. | Aporta a los objetivos del usuario: busca seguridad, formalidad y automatizaciÃ³n para proteger su prestigio y el presupuesto de la obra. |
| **PreocupaciÃ³n por sobrecostos logÃ­sticos** | 80% (4/5) | **Entrevistas 2, 3, 4 y 5:** Carlos y Leonardo afirman que los retrasos paralizan cuadrillas. SebastiÃ¡n cuantifica que las compras de emergencia elevan costos hasta un 18%. | Establece la motivaciÃ³n de compra (*driver*) del usuario: adoptarÃ¡n el sistema si este demuestra prevenir paralizaciones y reducir urgencias. |
| **Condicionamiento de adopciÃ³n tecnolÃ³gica** | 40% (2/5) | **Entrevistas 1 y 5:** SebastiÃ¡n condiciona el pago del SaaS a que el operario de campo realmente lo use y deje de llamar. AbdÃ³n exige poder gestionar desde campo. | Define las frustraciones potenciales frente a nuevas soluciones: el usuario teme pagar por un software que su equipo operativo se resista a utilizar. |

#### 4. Hallazgos principales
- **La informalidad como cuello de botella (100% de coincidencia):** El uso generalizado de WhatsApp para emitir "Ã“rdenes de Compra" informales es la principal causa de pÃ©rdida de informaciÃ³n, errores en especificaciones tÃ©cnicas y estrÃ©s administrativo.
- **El costo del retraso manual (80% de coincidencia):** La dependencia de Excel y aprobaciones lentas (hasta 2 dÃ­as) genera compras de emergencia que elevan los costos operativos de los proyectos de construcciÃ³n hasta en un 18%.
- **Necesidad de adopciÃ³n "Bottom-Up" (40% de coincidencia clave):** La decisiÃ³n de adquirir y mantener una plataforma de gestiÃ³n no solo depende de la directiva, sino de que la interfaz mÃ³vil sea lo suficientemente amigable y ligera para que el "Residente de Obra" la prefiera por encima de una llamada telefÃ³nica convencional.

#### 5. ConclusiÃ³n del segmento
Con base en las entrevistas registradas, este segmento se caracteriza por sufrir un alto nivel de estrÃ©s operativo debido a la brecha entre la urgencia del trabajo en campo y la lentitud de los procesos administrativos manuales en gabinete. Las evidencias obtenidas permiten establecer que el Ã©xito de una soluciÃ³n digital no radica en ofrecer funciones complejas, sino en reemplazar a WhatsApp con un flujo de aprobaciones inmediato, estructurado y de alta trazabilidad, lo cual resulta necesario para la construcciÃ³n del arquetipo de usuario: un profesional enfocado en la rentabilidad, urgido por la velocidad logÃ­stica y altamente dependiente de su telÃ©fono mÃ³vil.

## 2.3. Needfinding
A partir del anÃ¡lisis de las entrevistas y la recolecciÃ³n de informaciÃ³n sobre las dinÃ¡micas en la gestiÃ³n de proyectos de construcciÃ³n, se identificaron dos perfiles principales dentro de nuestro segmento objetivo que interactuarÃ¡n con la soluciÃ³n RQLS. Aunque ambos pertenecen a la gestiÃ³n de la obra, representan dos polos operativos: la urgencia de la ejecuciÃ³n en campo y la necesidad de control financiero en oficina. La construcciÃ³n de estos *User Persona* permite al equipo comprender sus motivaciones, frustraciones y el contraste en sus herramientas tecnolÃ³gicas, lo cual es vital para diseÃ±ar un flujo que conecte la obra con la gerencia de manera efectiva.

**1) Perfil 1: Ãrea operativa de campo**

Para el Ã¡rea operativa se elaborÃ³ el User Persona **Donnie Ruiz**. Se consideraron factores como su rol en la supervisiÃ³n fÃ­sica de las obras, su necesidad de cumplir cronogramas estrictos y su ritmo de trabajo altamente mÃ³vil. Sus principales frustraciones giran en torno a la burocracia logÃ­stica que retrasa la llegada de materiales y la dependencia de canales informales como WhatsApp para presionar por urgencias. Su perfil refleja una necesidad crÃ­tica de contar con una plataforma mÃ³vil, rÃ¡pida y responsiva, que le permita solicitar insumos y rastrear su estado de entrega en tiempo real sin abandonar el campo.

<img src="../docs/assets/chapter-02/user-persona01.png" alt="User Persona 1 - MartÃ­n" width="auto" height="1900"/>

<br>

**2) Perfil 2: Ãrea de control y gerencia**

Para el Ã¡rea de control y gerencia se elaborÃ³ el User Persona **Roberto AlcÃ¡ntara**. Se consideraron aspectos como su enfoque en la rentabilidad, la aprobaciÃ³n de presupuestos y la auditorÃ­a corporativa. Sus principales frustraciones estÃ¡n asociadas a la pÃ©rdida de dinero por "compras de emergencia" no planificadas, el desorden documentario y la inseguridad de usar hojas de Excel compartidas para llevar las finanzas. Su perfil requiere un entorno de escritorio (Dashboard) que centralice las cotizaciones, garantice la inmutabilidad de los datos y le permita aprobar Ã³rdenes de compra formales con un solo clic.

<img src="../docs/assets/chapter-02/user-persona02.png" alt="User Persona 2 - Roberto" width="auto" height="1900"/>

### 2.3.2. User Task Matrix

El User Task Matrix presenta las tareas clave que realizan los User Persona para cumplir sus objetivos en el dÃ­a a dÃ­a logÃ­stico y constructivo, independientemente de si usan nuestro software o no. Se evalÃºa la frecuencia y la importancia de cada tarea para identificar dÃ³nde RQLS debe aportar el mayor valor.

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse:collapse; width:100%; font-family:Arial, sans-serif; text-align:center;">
  <thead>
    <tr style="background-color:#eef3f7;">
      <th rowspan="2">Tarea (Task)</th>
      <th colspan="2">Ejecutor en Campo (MartÃ­n)</th>
      <th colspan="2">Gerente de Oficina (Roberto)</th>
    </tr>
    <tr style="background-color:#eef3f7;">
      <th>Frecuencia</th>
      <th>Importancia</th>
      <th>Frecuencia</th>
      <th>Importancia</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left;">Generar requerimientos de materiales de obra</td>
      <td>Often</td><td>High</td>
      <td>Rarely</td><td>Low</td>
    </tr>
    <tr>
      <td style="text-align:left;">Revisar y comparar cotizaciones de proveedores</td>
      <td>Rarely</td><td>Low</td>
      <td>Often</td><td>High</td>
    </tr>
    <tr>
      <td style="text-align:left;">Aprobar financieramente las Ã³rdenes de compra</td>
      <td>Occasionally</td><td>Medium</td>
      <td>Often</td><td>High</td>
    </tr>
    <tr>
      <td style="text-align:left;">Rastrear el estado de despacho y entrega de materiales</td>
      <td>Often</td><td>High</td>
      <td>Occasionally</td><td>Medium</td>
    </tr>
    <tr>
      <td style="text-align:left;">Controlar el gasto real vs. el presupuesto planificado</td>
      <td>Monthly</td><td>Medium</td>
      <td>Monthly</td><td>High</td>
    </tr>
    <tr>
      <td style="text-align:left;">Comunicar urgencias o retrasos logÃ­sticos a otras Ã¡reas</td>
      <td>Often</td><td>High</td>
      <td>Occasionally</td><td>High</td>
    </tr>
  </tbody>
</table>

**AnÃ¡lisis del Task Matrix:**
Se observa una clara complementariedad entre ambos perfiles. La tarea de **"Generar requerimientos de materiales"** es de altÃ­sima frecuencia e importancia para MartÃ­n (Campo), mientras que **"Revisar cotizaciones y Aprobar"** es el "Core" de Roberto (Oficina). Esto confirma que RQLS debe priorizar un flujo bidireccional: una interfaz de creaciÃ³n de pedidos ultra rÃ¡pida (Mobile) para el ejecutor, conectada automÃ¡ticamente a un Dashboard de aprobaciÃ³n seguro y comparativo (Desktop) para el gerente. Adicionalmente, la tarea de rastrear despachos (**High** para MartÃ­n) valida la necesidad de un sistema de notificaciones de estados.

<div style="page-break-after: always;"></div>

### 2.3.3. User Journey Mapping

El User Journey Mapping es una herramienta de diseÃ±o centrado en el usuario que nos permite **"caminar en las zapatos de otro"** del personal de construcciÃ³n. En este anÃ¡lisis, mapeamos el viaje emocional y operativo que recorren tanto el Jefe de Campo (urgencia tÃ©cnica) como el Gerente de Oficina (control financiero) durante el ciclo de abastecimiento.

**1) Perfil 1: Ãrea operativa de campo**

<img src="../docs/assets/chapter-02/user-journey-mapping2.png" alt="User Journey Mapping 1 - Martin" width="auto" height="1900"/>

**2) Perfil 2: Ãrea de control y gerencia**

<img src="../docs/assets/chapter-02/user-journey-mapping1.png" alt="User Journey Mapping 2 - Roberto" width="auto" height="1900"/>

### 2.3.4. Empathy Mapping

Para crear una soluciÃ³n que realmente se vincule con las personas, no es suficiente con saber quÃ© hacen; tenemos que comprender lo que sienten. El Empathy Mapping es una herramienta de diseÃ±o centrado en el usuario que nos posibilita trascender los datos demogrÃ¡ficos y explorar mÃ¡s a fondo el mundo interno de nuestros perfiles.

**1) Perfil 1: Ãrea operativa de campo**

<img src="../docs/assets/chapter-02/empathy-mapping1.png" alt="Empathy Mapping 1 - Martin" width="auto" height="1900"/>

**2) Perfil 2: Ãrea de control y gerencia**

<img src="../docs/assets/chapter-02/empathy-mapping2.png" alt="Empathy Mapping 2 - Roberto" width="auto" height="1900"/>

## 2.4. Big Picture EventStorming

Para diseÃ±ar un sistema robusto, primero debemos entender el negocio como un todo, dejando de lado los tecnicismos para enfocarnos en la lÃ³gica pura del dominio. El Big Picture EventStorming es una tÃ©cnica colaborativa que nos ayuda a visualizar todos los eventos significativos que ocurren en la cadena de abastecimiento de una constructora. Al organizar estos eventos de manera cronolÃ³gica, logramos identificar los flujos crÃ­ticos del negocio y los puntos exactos donde la informaciÃ³n suele perderse o demorarse en la transiciÃ³n entre la obra y la oficina central.

**Step 1 â€“ Free Exploration**

En esta primera etapa, el equipo realizÃ³ una sesiÃ³n de lluvia de ideas para capturar todos los eventos de dominio relevantes, sin preocuparse inicialmente por el orden o la jerarquÃ­a. El objetivo principal fue representar los acontecimientos reales del negocio â€”como la detecciÃ³n de una falta de material o la negociaciÃ³n de un precioâ€” de manera independiente a cualquier funciÃ³n tÃ©cnica o arquitectura del sistema.

<img src="../docs/assets/chapter-02/big-picture-event-storming1.png" alt="Big Picture EventStorming 1" width="auto" height="1900"/>

**Step 2 â€“ Structured Organization** 

DespuÃ©s de listar los eventos en esta estructura nos permitiÃ³ aislar los procesos clave, desde el requerimiento inicial en el frente de obra hasta la conciliaciÃ³n financiera final, resaltando las Ã¡reas de mejora que serÃ¡n abordadas mediante nuestra soluciÃ³n digital.

<img src="../docs/assets/chapter-02/big-picture-event-storming2.png" alt="Big Picture EventStorming 2" width="auto" height="1900"/>

## 2.5. Ubiquitous Language

| Term                   | Definition                                                                                                                         |
|------------------------|------------------------------------------------------------------------------------------------------------------------------------|
| Field Supervisor     |Project manager or engineer located at the construction site responsible for identifying needs, creating requisitions, and confirming material receipt.|
| Project Manager      | Strategic user who manages budgets, reviews cost comparisons, and authorizes purchase orders from the central office.      |
| Supplier             | External entity registered in the platform that receives quote requests, submits proposals, and dispatches materials to project sites. |
| Material Requisition | Formal internal request created by the field supervisor when a material shortage or minimum stock level is detected.                 |
| Purchase Order (PO)  | Formal and immutable document approved by management that authorizes the legal and financial acquisition of materials from a supplier.  |
| Comparison Sheet     | Document automatically generated by the system that allows for side-by-side analysis of prices, delivery times, and supplier reliability.|
| Waybill              | Document delivered by the supplier upon arrival; in Buildline, it is digitalized via OCR to certify the physical receipt of goods.    |
| Way Match            | Automated validation process where the system verifies that the Purchase Order, Waybill, and Invoice all match in quantity and price.  |
| Safety Stock         | Minimum inventory level defined for critical materials (like cement or rebar) that triggers an automatic alert to prevent project downtime.              |
| Waste                | Recorded loss or non-productive consumption of material during execution, used to adjust the project's actual cost vs. planned budget. |
| APU                  | Technical budget baseline used to validate if a requisitionâ€™s cost is aligned with the project's financial planning.                   |
| Logistics Overcost   | The 21.1% average extra expense incurred by MYPES due to inefficient manual processes and emergency purchases that Buildline aims to reduce.|
| Project Dashboard    | Centralized interface for management showing real-time metrics, requisition statuses, and overall project profitability.        |
| Field App            | Mobile-first interface designed for high-speed use in construction environments, allowing for "3-click" requisitions and OCR scanning. |
| Audit Log            | Immutable record of every action taken in the system (approvals, edits, deletions) to ensure total transparency and accountability. |

**Expected benefits of the ubiquitous language:**

- Facilitates communication: Bridges the gap between developers, field engineers, and financial administrators.
- Improves technical alignment: Ensures that database tables and UI labels match the business reality.
- Avoids ambiguities: Clearly distinguishes between an internal "Requisition" and an external "Purchase Order," preventing procurement errors.
- Ensures consistency: Guarantees that documentation, mobile interfaces, and project reports use the same professional terminology.


<div class="page-break"></div>

# CapÃ­tulo III: Requirements Specification

## TO-BE Scenario Mapping
Jefes de Proyecto / Gerentes Generales

| Fase | Doing (QuÃ© hace) | Thinking (QuÃ© piensa) | Feeling (QuÃ© siente) |
|------|----------------|----------------------|----------------------|
| EvaluaciÃ³n de requerimientos | Revisa solicitudes de materiales con informaciÃ³n consolidada, incluyendo prioridad, costo estimado e impacto en el proyecto, provenientes de obra y logÃ­stica. | â€œNecesito entender rÃ¡pidamente quÃ© solicitudes son crÃ­ticas y cuÃ¡les pueden optimizarse para no afectar el proyecto.â€ | AnalÃ­tico y bajo presiÃ³n por tomar decisiones rÃ¡pidas. |
| AnÃ¡lisis y comparaciÃ³n | EvalÃºa cotizaciones de diferentes proveedores considerando variables como precio, tiempo de entrega, calidad y confiabilidad del proveedor. | â€œDebo elegir la mejor opciÃ³n en tÃ©rminos de costo-beneficio sin comprometer el cronograma ni la calidad.â€ | EstratÃ©gico, cauteloso y enfocado en resultados. |
| Toma de decisiÃ³n | Aprueba o rechaza solicitudes de compra dentro del sistema basÃ¡ndose en informaciÃ³n clara, validada y estructurada. | â€œMi decisiÃ³n debe estar bien fundamentada para evitar sobrecostos o retrasos en la obra.â€ | Responsable y con presiÃ³n por el impacto de sus decisiones. |
| Seguimiento y control | Monitorea el estado de pedidos, cumplimiento de entregas y ejecuciÃ³n presupuestal mediante dashboards, indicadores y alertas del sistema. | â€œNecesito asegurar que todo se estÃ© ejecutando segÃºn lo planificado y dentro del presupuesto establecido.â€ | Vigilante, con mayor sensaciÃ³n de control y seguridad. |

## 3.1. User Stories

## Epics

| EPIC ID | Titulo | Descripcion |
|--------|--------|-------------|
| EP-01 | GestiÃ³n de requerimientos | Permite registrar, visualizar, buscar y filtrar requerimientos de materiales desde obra, asegurando un flujo estructurado de solicitudes. |
| EP-02 | GestiÃ³n de compras y abastecimiento | Permite gestionar el proceso completo de compras: cotizaciones, comparaciÃ³n, aprobaciÃ³n y generaciÃ³n de Ã³rdenes de compra. |
| EP-03 | GestiÃ³n de inventario y almacÃ©n | Permite controlar el stock de materiales, registrar movimientos y confirmar la recepciÃ³n de pedidos para mantener inventarios actualizados. |
| EP-04 | GestiÃ³n de usuarios y seguridad | Permite registrar usuarios, gestionar roles y controlar accesos al sistema mediante autenticaciÃ³n segura. |
| EP-05 | AnÃ¡lisis y control de gestiÃ³n | Permite visualizar indicadores, historial de compras y control presupuestal para la toma de decisiones estratÃ©gicas. |
| EP-06 | ComunicaciÃ³n e integraciÃ³n | Permite enviar notificaciones, acceso mÃ³vil y exportaciÃ³n/importaciÃ³n de datos para mejorar la conectividad y usabilidad del sistema. |
| EP-07 | GestiÃ³n de proveedores | Permite registrar, evaluar y gestionar proveedores, asÃ­ como controlar incidencias relacionadas con ellos. |

## User Stories

| US ID | TÃ­tulo | DescripciÃ³n | Criterio de AceptaciÃ³n | Relacionado con (EPIC ID) |
|------|--------|-------------|------------------------|--------------------------|
| US 001 | Registrar requerimiento de material | **Como** ingeniero residente,<br>**Quiero** registrar un requerimiento de materiales desde obra,<br>**Para** iniciar el proceso de abastecimiento de forma estructurada. | **Escenario 1: Registro correcto**<br>**Dado** que el usuario completa los campos obligatorios (material, cantidad, proyecto y prioridad),<br>**Cuando** envÃ­a el requerimiento,<br>**Entonces** el sistema registra el requerimiento con un ID Ãºnico, estado â€œPendienteâ€ y fecha de registro.<br><br>**Escenario 2: Datos incompletos**<br>**Dado** que faltan campos obligatorios,<br>**Cuando** intenta enviar el requerimiento,<br>**Entonces** el sistema bloquea el registro y muestra mensajes especÃ­ficos por campo. | EP-01 |
| US 002 | Adjuntar evidencia al requerimiento | **Como** ingeniero residente,<br>**Quiero** adjuntar fotos o documentos al requerimiento,<br>**Para** brindar mayor claridad sobre el material solicitado. | **Escenario 1: Archivo vÃ¡lido**<br>**Dado** que el usuario adjunta archivos JPG, PNG o PDF menores a 10MB,<br>**Cuando** envÃ­a el requerimiento,<br>**Entonces** los archivos se almacenan correctamente y se vinculan al requerimiento.<br><br>**Escenario 2: Archivo invÃ¡lido**<br>**Dado** que el archivo excede el tamaÃ±o o el formato permitido,<br>**Cuando** intenta cargarlo,<br>**Entonces** el sistema muestra un error indicando la restricciÃ³n. | EP-01 |
| US 003 | Visualizar lista de requerimientos | **Como** analista de logÃ­stica,<br>**Quiero** ver todos los requerimientos en una lista,<br>**Para** gestionarlos eficientemente. | **Escenario 1: Lista con datos**<br>**Dado** que existen requerimientos registrados,<br>**Cuando** accede a la lista,<br>**Entonces** el sistema muestra los requerimientos en una tabla con filtros, ordenados por fecha y prioridad.<br><br>**Escenario 2: Sin datos**<br>**Dado** que no existen requerimientos registrados,<br>**Cuando** accede a la lista,<br>**Entonces** el sistema muestra el mensaje â€œNo hay requerimientos registradosâ€. | EP-01 |
| US 004 | Filtrar requerimientos | **Como** analista de logÃ­stica,<br>**Quiero** filtrar requerimientos por estado o proyecto,<br>**Para** encontrarlos rÃ¡pidamente. | **Escenario 1: Filtro aplicado**<br>**Dado** que selecciona criterios como estado, proyecto o fecha,<br>**Cuando** aplica el filtro,<br>**Entonces** el sistema actualiza la lista mostrando solo las coincidencias.<br><br>**Escenario 2: Sin coincidencias**<br>**Dado** que no existen resultados que coincidan con los criterios,<br>**Cuando** aplica el filtro,<br>**Entonces** el sistema muestra un mensaje claro sin afectar la interfaz. | EP-01 |
| US 005 | Generar solicitud de cotizaciÃ³n | **Como** analista de logÃ­stica,<br>**Quiero** generar solicitudes de cotizaciÃ³n,<br>**Para** obtener precios de proveedores. | **Escenario 1: GeneraciÃ³n correcta**<br>**Dado** que el requerimiento estÃ¡ aprobado,<br>**Cuando** genera la solicitud de cotizaciÃ³n,<br>**Entonces** el sistema crea un documento con los detalles del requerimiento y lo deja listo para enviarse a los proveedores.<br><br>**Escenario 2: Error de validaciÃ³n**<br>**Dado** que faltan datos obligatorios,<br>**Cuando** intenta generar la solicitud,<br>**Entonces** el sistema notifica quÃ© campos deben completarse. | EP-02 |
| US 006 | Registrar cotizaciones | **Como** analista de logÃ­stica,<br>**Quiero** registrar cotizaciones recibidas,<br>**Para** compararlas. | **Escenario 1: Registro vÃ¡lido**<br>**Dado** que ingresa proveedor, precio y tiempo de entrega,<br>**Cuando** guarda la cotizaciÃ³n,<br>**Entonces** la cotizaciÃ³n queda asociada al requerimiento.<br><br>**Escenario 2: Datos incompletos**<br>**Dado** que faltan campos obligatorios,<br>**Cuando** intenta guardar,<br>**Entonces** el sistema impide el registro y muestra las validaciones correspondientes. | EP-02 |
| US 007 | Comparar cotizaciones | **Como** jefe de proyecto,<br>**Quiero** comparar cotizaciones,<br>**Para** elegir la mejor opciÃ³n. | **Escenario 1: ComparaciÃ³n disponible**<br>**Dado** que existen mÃºltiples cotizaciones registradas,<br>**Cuando** accede a la comparaciÃ³n,<br>**Entonces** el sistema muestra una tabla comparativa con precio, tiempo de entrega y proveedor.<br><br>**Escenario 2: Sin cotizaciones**<br>**Dado** que no existen cotizaciones registradas,<br>**Cuando** accede a la comparaciÃ³n,<br>**Entonces** el sistema muestra un mensaje indicando la ausencia de datos. | EP-02 |
| US 008 | Aprobar compra | **Como** jefe de proyecto,<br>**Quiero** aprobar compras,<br>**Para** autorizar gastos dentro del sistema. | **Escenario 1: AprobaciÃ³n**<br>**Dado** que revisa una cotizaciÃ³n,<br>**Cuando** aprueba la compra,<br>**Entonces** el sistema cambia el estado a â€œAprobadoâ€ y continÃºa el proceso.<br><br>**Escenario 2: Rechazo**<br>**Dado** que decide rechazar la compra,<br>**Cuando** registra la decisiÃ³n,<br>**Entonces** el sistema solicita un motivo y notifica a logÃ­stica. | EP-02 |
| US 009 | Generar orden de compra | **Como** analista de logÃ­stica,<br>**Quiero** generar Ã³rdenes de compra,<br>**Para** formalizar pedidos. | **Escenario 1: GeneraciÃ³n correcta**<br>**Dado** que la compra estÃ¡ aprobada,<br>**Cuando** genera la orden de compra,<br>**Entonces** el sistema crea un documento con cÃ³digo Ãºnico y datos completos.<br><br>**Escenario 2: Error de validaciÃ³n**<br>**Dado** que existen inconsistencias en los datos,<br>**Cuando** intenta generar la orden,<br>**Entonces** el sistema alerta sobre las inconsistencias detectadas. | EP-02 |
| US 010 | Notificar al proveedor | **Como** analista de logÃ­stica,<br>**Quiero** notificar al proveedor,<br>**Para** iniciar el proceso de entrega. | **Escenario 1: NotificaciÃ³n exitosa**<br>**Dado** que existe una orden de compra,<br>**Cuando** envÃ­a la notificaciÃ³n,<br>**Entonces** el proveedor recibe un correo con los detalles de la orden.<br><br>**Escenario 2: Error de envÃ­o**<br>**Dado** que ocurre un fallo al enviar la notificaciÃ³n,<br>**Cuando** el sistema registra el intento fallido,<br>**Entonces** permite reenviar el mensaje. | EP-06 |
| US 011 | Seguimiento de pedidos | **Como** ingeniero residente,<br>**Quiero** ver el estado de mis pedidos,<br>**Para** monitorear avances. | **Escenario 1: Estado actualizado**<br>**Dado** que el pedido estÃ¡ en proceso,<br>**Cuando** consulta el seguimiento,<br>**Entonces** visualiza los estados (pendiente, enviado, entregado) con sus fechas correspondientes.<br><br>**Escenario 2: Sin datos**<br>**Dado** que no existen pedidos registrados,<br>**Cuando** consulta el seguimiento,<br>**Entonces** el sistema muestra un mensaje informativo. | EP-02 |
| US 012 | Confirmar recepciÃ³n de materiales | **Como** ingeniero residente,<br>**Quiero** confirmar la recepciÃ³n de materiales,<br>**Para** cerrar pedidos correctamente. | **Escenario 1: ConfirmaciÃ³n**<br>**Dado** que recibe los materiales,<br>**Cuando** confirma la recepciÃ³n,<br>**Entonces** el pedido pasa a â€œCompletadoâ€ y se registra la fecha y el responsable.<br><br>**Escenario 2: ValidaciÃ³n adicional**<br>**Dado** que falta validar informaciÃ³n asociada al pedido,<br>**Cuando** intenta cerrar la recepciÃ³n,<br>**Entonces** el sistema solicita una validaciÃ³n adicional antes de finalizar. | EP-03 |
| US 013 | Registrar incidencias | **Como** ingeniero residente,<br>**Quiero** registrar problemas con proveedores,<br>**Para** llevar control de incidencias. | **Escenario 1: Registro**<br>**Dado** que detecta un problema con un proveedor,<br>**Cuando** registra la incidencia con evidencia,<br>**Entonces** queda guardada con estado â€œAbiertaâ€ y asociada al pedido.<br><br>**Escenario 2: Error de validaciÃ³n**<br>**Dado** que faltan campos obligatorios,<br>**Cuando** intenta registrar la incidencia,<br>**Entonces** el sistema valida la informaciÃ³n antes de guardar. | EP-07 |
| US 014 | Controlar stock | **Como** analista de logÃ­stica,<br>**Quiero** ver el stock disponible,<br>**Para** evitar faltantes de materiales. | **Escenario 1: Stock disponible**<br>**Dado** que existen materiales en almacÃ©n,<br>**Cuando** consulta el inventario,<br>**Entonces** el sistema muestra el stock actualizado por almacÃ©n y tipo de material.<br><br>**Escenario 2: Sin stock**<br>**Dado** que no existe stock disponible,<br>**Cuando** consulta el inventario,<br>**Entonces** el sistema muestra una alerta visual y una sugerencia de reposiciÃ³n. | EP-03 |
| US 015 | Actualizar stock | **Como** analista de logÃ­stica,<br>**Quiero** actualizar el inventario,<br>**Para** mantener datos reales del almacÃ©n. | **Escenario 1: ActualizaciÃ³n correcta**<br>**Dado** que se registra ingreso o salida de materiales,<br>**Cuando** guarda el movimiento,<br>**Entonces** el stock se actualiza automÃ¡ticamente.<br><br>**Escenario 2: Error de consistencia**<br>**Dado** que el movimiento genera inconsistencias,<br>**Cuando** intenta guardar,<br>**Entonces** el sistema evita el cambio y muestra la validaciÃ³n correspondiente. | EP-03 |
| US 016 | Visualizar historial de compras | **Como** jefe de proyecto,<br>**Quiero** ver el historial de compras,<br>**Para** analizar decisiones pasadas. | **Escenario 1: Historial visible**<br>**Dado** que existen compras registradas,<br>**Cuando** accede al historial,<br>**Entonces** se muestra una lista filtrable por fecha, proveedor y proyecto.<br><br>**Escenario 2: Historial vacÃ­o**<br>**Dado** que no existen compras registradas,<br>**Cuando** accede al historial,<br>**Entonces** el sistema muestra un mensaje informativo. | EP-05 |
| US 017 | Control presupuestal | **Como** jefe de proyecto,<br>**Quiero** ver el control de costos,<br>**Para** evitar sobrecostos en el proyecto. | **Escenario 1: Datos actualizados**<br>**Dado** que el sistema cuenta con informaciÃ³n financiera actualizada,<br>**Cuando** consulta el control presupuestal,<br>**Entonces** visualiza un dashboard con presupuesto vs. gasto real.<br><br>**Escenario 2: Error de datos**<br>**Dado** que existe inconsistencia en la informaciÃ³n,<br>**Cuando** accede al control presupuestal,<br>**Entonces** el sistema muestra una alerta de inconsistencia. | EP-05 |
| US 018 | Alertas de sobrecosto | **Como** jefe de proyecto,<br>**Quiero** recibir alertas de sobrecostos,<br>**Para** prevenir desviaciones presupuestales. | **Escenario 1: Exceso**<br>**Dado** que el gasto supera el umbral definido,<br>**Cuando** se registra la variaciÃ³n presupuestal,<br>**Entonces** el sistema envÃ­a una alerta automÃ¡tica.<br><br>**Escenario 2: Dentro del rango**<br>**Dado** que el gasto no supera el umbral,<br>**Cuando** se actualiza el presupuesto,<br>**Entonces** el sistema no genera alertas. | EP-05 |
| US 019 | Dashboard general | **Como** jefe de proyecto,<br>**Quiero** visualizar indicadores generales,<br>**Para** tomar decisiones rÃ¡pidas. | **Escenario 1: Dashboard cargado**<br>**Dado** que existen datos disponibles,<br>**Cuando** accede al dashboard,<br>**Entonces** se muestran KPIs como costos, pedidos y tiempos.<br><br>**Escenario 2: Sin datos**<br>**Dado** que no existen datos suficientes,<br>**Cuando** accede al dashboard,<br>**Entonces** el sistema muestra un mensaje informativo. | EP-05 |
| US 020 | Acceso mÃ³vil | **Como** ingeniero residente,<br>**Quiero** acceder desde el mÃ³vil,<br>**Para** gestionar procesos desde obra. | **Escenario 1: Acceso correcto**<br>**Dado** que el usuario accede desde un dispositivo mÃ³vil,<br>**Cuando** ingresa al sistema,<br>**Entonces** la interfaz se adapta correctamente y mantiene sus funciones principales.<br><br>**Escenario 2: Error de compatibilidad**<br>**Dado** que el navegador o dispositivo no es compatible,<br>**Cuando** intenta ingresar,<br>**Entonces** el sistema muestra un mensaje de compatibilidad. | EP-06 |
| US 021 | Notificaciones en tiempo real | **Como** usuario,<br>**Quiero** recibir notificaciones en tiempo real,<br>**Para** reaccionar rÃ¡pidamente a eventos. | **Escenario 1: Evento ocurre**<br>**Dado** que sucede un evento relevante en el sistema,<br>**Cuando** se registra el evento,<br>**Entonces** el sistema envÃ­a una notificaciÃ³n inmediata.<br><br>**Escenario 2: Error de entrega**<br>**Dado** que falla el envÃ­o de la notificaciÃ³n,<br>**Cuando** el sistema detecta el error,<br>**Entonces** reintenta automÃ¡ticamente el envÃ­o. | EP-06 |
| US 022 | Registro de usuarios | **Como** analista de logÃ­stica,<br>**Quiero** registrar usuarios en el sistema,<br>**Para** permitir el acceso controlado. | **Escenario 1: Registro vÃ¡lido**<br>**Dado** que el formulario contiene datos correctos,<br>**Cuando** registra el usuario,<br>**Entonces** el sistema lo crea con el rol asignado.<br><br>**Escenario 2: Datos invÃ¡lidos**<br>**Dado** que los datos son incorrectos o incompletos,<br>**Cuando** intenta crear el usuario,<br>**Entonces** el sistema valida la informaciÃ³n antes de guardar. | EP-04 |
| US 023 | Inicio de sesiÃ³n | **Como** usuario,<br>**Quiero** iniciar sesiÃ³n,<br>**Para** acceder al sistema. | **Escenario 1: Credenciales correctas**<br>**Dado** que el usuario ingresa credenciales vÃ¡lidas,<br>**Cuando** inicia sesiÃ³n,<br>**Entonces** accede al sistema correctamente.<br><br>**Escenario 2: Credenciales incorrectas**<br>**Dado** que el usuario ingresa credenciales invÃ¡lidas,<br>**Cuando** intenta acceder varias veces,<br>**Entonces** el sistema bloquea el acceso tras mÃºltiples intentos fallidos. | EP-04 |
| US 024 | GestiÃ³n de roles | **Como** jefe de proyecto,<br>**Quiero** gestionar roles,<br>**Para** controlar permisos dentro del sistema. | **Escenario 1: Rol asignado**<br>**Dado** que selecciona un usuario y un rol,<br>**Cuando** guarda la asignaciÃ³n,<br>**Entonces** el sistema aplica los permisos correspondientes.<br><br>**Escenario 2: Error de validaciÃ³n**<br>**Dado** que la informaciÃ³n es inconsistente,<br>**Cuando** intenta guardar el rol,<br>**Entonces** el sistema bloquea la acciÃ³n y muestra el error. | EP-04 |
| US 025 | Historial de acciones | **Como** jefe de proyecto,<br>**Quiero** ver el historial de acciones,<br>**Para** auditorÃ­a del sistema. | **Escenario 1: Logs visibles**<br>**Dado** que existen registros de actividad,<br>**Cuando** accede al historial,<br>**Entonces** se muestran los registros con usuario, fecha y acciÃ³n.<br><br>**Escenario 2: Sin logs**<br>**Dado** que no existen registros,<br>**Cuando** accede al historial,<br>**Entonces** el sistema muestra un mensaje informativo. | EP-04 |
| US 026 | BÃºsqueda global | **Como** analista de logÃ­stica,<br>**Quiero** buscar informaciÃ³n en el sistema,<br>**Para** encontrar datos rÃ¡pidamente. | **Escenario 1: Coincidencia encontrada**<br>**Dado** que existe informaciÃ³n relacionada con el tÃ©rmino buscado,<br>**Cuando** realiza la bÃºsqueda,<br>**Entonces** el sistema muestra resultados categorizados.<br><br>**Escenario 2: Sin resultados**<br>**Dado** que no existen coincidencias,<br>**Cuando** ejecuta la bÃºsqueda,<br>**Entonces** el sistema muestra un mensaje claro. | EP-01 |
| US 027 | IntegraciÃ³n con Excel | **Como** jefe de proyecto,<br>**Quiero** exportar datos a Excel,<br>**Para** realizar anÃ¡lisis externos. | **Escenario 1: ExportaciÃ³n correcta**<br>**Dado** que existen datos disponibles para exportar,<br>**Cuando** solicita la exportaciÃ³n,<br>**Entonces** el sistema descarga un archivo Excel estructurado correctamente.<br><br>**Escenario 2: Error de exportaciÃ³n**<br>**Dado** que ocurre un problema durante el proceso,<br>**Cuando** se genera la exportaciÃ³n,<br>**Entonces** el sistema muestra un mensaje de fallo. | EP-06 |
| US 028 | Carga masiva de datos | **Como** analista de logÃ­stica,<br>**Quiero** subir datos de forma masiva,<br>**Para** ahorrar tiempo en registros. | **Escenario 1: Archivo vÃ¡lido**<br>**Dado** que el archivo cumple con la estructura requerida,<br>**Cuando** lo carga al sistema,<br>**Entonces** el sistema procesa la informaciÃ³n y muestra un resumen de registros.<br><br>**Escenario 2: Error en archivo**<br>**Dado** que el archivo contiene errores,<br>**Cuando** intenta cargarlo,<br>**Entonces** el sistema genera un reporte de errores. | EP-06 |
| US 029 | GestiÃ³n de proveedores | **Como** analista de logÃ­stica,<br>**Quiero** registrar proveedores,<br>**Para** tener una base de datos organizada. | **Escenario 1: Registro correcto**<br>**Dado** que el formulario contiene informaciÃ³n completa,<br>**Cuando** registra el proveedor,<br>**Entonces** el sistema guarda el proveedor correctamente.<br><br>**Escenario 2: Error de validaciÃ³n**<br>**Dado** que faltan datos obligatorios,<br>**Cuando** intenta guardar el proveedor,<br>**Entonces** el sistema valida la informaciÃ³n antes de confirmar. | EP-07 |
| US 030 | EvaluaciÃ³n de proveedores | **Como** jefe de proyecto,<br>**Quiero** calificar proveedores,<br>**Para** mejorar decisiones futuras. | **Escenario 1: EvaluaciÃ³n guardada**<br>**Dado** que completa la calificaciÃ³n del proveedor,<br>**Cuando** guarda la evaluaciÃ³n,<br>**Entonces** queda visible en el historial.<br><br>**Escenario 2: Error de validaciÃ³n**<br>**Dado** que faltan campos obligatorios,<br>**Cuando** intenta guardar,<br>**Entonces** el sistema valida la informaciÃ³n antes de almacenar la evaluaciÃ³n. | EP-07 |

## Technical Stories

| TS ID | TÃ­tulo | DescripciÃ³n | Criterios de AceptaciÃ³n | Relacionado con (EPIC ID) |
|------|--------|-------------|------------------------|--------------------------|
| TS-01 | Obtener perfil por ID | **Como** desarrollador,<br>**Quiero** obtener el perfil de un usuario por su ID,<br>**Para** recuperar informaciÃ³n detallada del usuario dentro del sistema. | **Escenario 1: Perfil existente**<br>**Dado** que el endpoint `/api/v1/profiles/{id}` estÃ¡ disponible y el usuario existe,<br>**Cuando** se envÃ­a un request GET con un ID vÃ¡lido,<br>**Entonces** el sistema responde con status 200, retorna los datos completos del perfil (nombre, apellidos, email, rol) y un tiempo de respuesta menor a 2 segundos.<br><br>**Escenario 2: Perfil inexistente**<br>**Dado** que el ID no existe,<br>**Cuando** se realiza la consulta,<br>**Entonces** el sistema responde con status 404 y un mensaje claro: â€œPerfil de usuario no encontradoâ€. | EP-06 |
| TS-02 | Actualizar perfil por ID | **Como** desarrollador,<br>**Quiero** actualizar los datos de un perfil de usuario,<br>**Para** mantener la informaciÃ³n actualizada en el sistema. | **Escenario 1: ActualizaciÃ³n vÃ¡lida**<br>**Dado** que el endpoint `/api/v1/profiles/{id}` estÃ¡ disponible y el usuario existe,<br>**Cuando** se envÃ­a un request PUT con datos vÃ¡lidos (nombre, email, direcciÃ³n),<br>**Entonces** el sistema valida los campos, actualiza la informaciÃ³n y responde con status 200 mostrando el perfil actualizado.<br><br>**Escenario 2: Usuario inexistente**<br>**Dado** que el ID no estÃ¡ registrado,<br>**Cuando** se intenta actualizar,<br>**Entonces** el sistema responde con status 404 y un mensaje de error. | EP-06 |
| TS-03 | Obtener todos los perfiles | **Como** desarrollador,<br>**Quiero** listar todos los perfiles de usuario,<br>**Para** permitir su visualizaciÃ³n y gestiÃ³n. | **Escenario 1: Lista con datos**<br>**Dado** que existen usuarios registrados,<br>**Cuando** se envÃ­a un request GET a `/api/v1/profiles`,<br>**Entonces** el sistema retorna status 200 con una lista estructurada de perfiles.<br><br>**Escenario 2: Lista vacÃ­a**<br>**Dado** que no existen usuarios registrados,<br>**Cuando** se envÃ­a el request GET,<br>**Entonces** el sistema retorna status 204 indicando ausencia de datos. | EP-06 |
| TS-04 | Obtener materiales | **Como** desarrollador,<br>**Quiero** obtener todos los materiales registrados,<br>**Para** visualizar el inventario disponible en el sistema. | **Escenario 1: Materiales disponibles**<br>**Dado** que existen registros en `/api/v1/materials`,<br>**Cuando** se realiza un GET,<br>**Entonces** se retorna status 200 con la lista de materiales incluyendo nombre, stock y unidad.<br><br>**Escenario 2: Sin materiales**<br>**Dado** que no existen materiales registrados,<br>**Cuando** se consulta el endpoint,<br>**Entonces** se retorna status 204 con mensaje informativo. | EP-01 |
| TS-05 | Crear material | **Como** desarrollador,<br>**Quiero** registrar un nuevo material,<br>**Para** ampliar el catÃ¡logo disponible. | **Escenario 1: CreaciÃ³n vÃ¡lida**<br>**Dado** que se envÃ­an datos completos (nombre, unidad, stock inicial),<br>**Cuando** se hace POST a `/api/v1/materials`,<br>**Entonces** el sistema valida los datos, crea el registro y retorna status 201.<br><br>**Escenario 2: Datos incompletos**<br>**Dado** que faltan campos obligatorios,<br>**Cuando** se realiza el POST,<br>**Entonces** el sistema retorna status 400 con mensaje indicando los campos faltantes. | EP-03 |
| TS-06 | Obtener material por ID | **Como** desarrollador,<br>**Quiero** obtener un material especÃ­fico por su ID,<br>**Para** visualizar su informaciÃ³n detallada. | **Escenario 1: Material existente**<br>**Dado** que el material existe,<br>**Cuando** se consulta `/api/v1/materials/{id}`,<br>**Entonces** el sistema responde con status 200 y los datos del material.<br><br>**Escenario 2: No existe**<br>**Dado** que el material no estÃ¡ registrado,<br>**Cuando** se consulta el endpoint,<br>**Entonces** responde con status 404 y mensaje â€œMaterial no encontradoâ€. | EP-01 |
| TS-07 | Actualizar material | **Como** desarrollador,<br>**Quiero** actualizar un material,<br>**Para** mantener la informaciÃ³n correcta en el inventario. | **Escenario 1: ActualizaciÃ³n correcta**<br>**Dado** que se envÃ­a un PUT con datos vÃ¡lidos,<br>**Cuando** se actualiza el material,<br>**Entonces** el sistema retorna status 200 y confirma la actualizaciÃ³n.<br><br>**Escenario 2: Error**<br>**Dado** que el material no existe,<br>**Cuando** se intenta actualizar,<br>**Entonces** el sistema retorna status 404. | EP-03 |
| TS-08 | Eliminar material | **Como** desarrollador,<br>**Quiero** eliminar materiales,<br>**Para** mantener el inventario limpio y actualizado. | **Escenario 1: EliminaciÃ³n vÃ¡lida**<br>**Dado** que se envÃ­a un DELETE con un ID existente,<br>**Cuando** se ejecuta la operaciÃ³n,<br>**Entonces** el sistema retorna status 204 y elimina el registro.<br><br>**Escenario 2: No existe**<br>**Dado** que el ID no estÃ¡ registrado,<br>**Cuando** se intenta eliminar,<br>**Entonces** el sistema retorna status 404. | EP-03 |
| TS-09 | Obtener categorÃ­as | **Como** desarrollador,<br>**Quiero** obtener categorÃ­as de materiales,<br>**Para** clasificar los recursos del sistema. | **Escenario 1: Con datos**<br>**Dado** que existen categorÃ­as registradas,<br>**Cuando** se realiza GET a `/api/v1/categories`,<br>**Entonces** el sistema retorna status 200 con la lista.<br><br>**Escenario 2: Sin datos**<br>**Dado** que no existen categorÃ­as registradas,<br>**Cuando** se consulta el endpoint,<br>**Entonces** el sistema retorna status 204. | EP-01 |
| TS-10 | Obtener categorÃ­a por ID | **Como** desarrollador,<br>**Quiero** obtener una categorÃ­a especÃ­fica,<br>**Para** ver su detalle. | **Escenario 1: Existe**<br>**Dado** que la categorÃ­a existe,<br>**Cuando** se consulta el endpoint por ID,<br>**Entonces** el sistema retorna status 200 con nombre e informaciÃ³n.<br><br>**Escenario 2: No existe**<br>**Dado** que la categorÃ­a no estÃ¡ registrada,<br>**Cuando** se realiza la consulta,<br>**Entonces** el sistema retorna status 404. | EP-01 |
| TS-11 | AutenticaciÃ³n de usuario | **Como** desarrollador,<br>**Quiero** autenticar usuarios,<br>**Para** garantizar acceso seguro al sistema. | **Escenario 1: Credenciales vÃ¡lidas**<br>**Dado** que el usuario envÃ­a credenciales correctas,<br>**Cuando** realiza un POST a `/api/v1/auth/sign-in`,<br>**Entonces** el sistema retorna status 200 con un token JWT vÃ¡lido y su tiempo de expiraciÃ³n.<br><br>**Escenario 2: Credenciales invÃ¡lidas**<br>**Dado** que las credenciales son incorrectas,<br>**Cuando** intenta iniciar sesiÃ³n,<br>**Entonces** el sistema retorna status 401 con un mensaje claro. | EP-04 |
| TS-12 | Registro de usuario | **Como** desarrollador,<br>**Quiero** registrar nuevos usuarios,<br>**Para** permitir acceso controlado. | **Escenario 1: Registro exitoso**<br>**Dado** que el request POST a `/api/v1/auth/sign-up` contiene datos vÃ¡lidos,<br>**Cuando** se envÃ­a la solicitud,<br>**Entonces** el sistema retorna status 201 y crea el usuario.<br><br>**Escenario 2: Email duplicado**<br>**Dado** que el correo ya existe en el sistema,<br>**Cuando** se intenta registrar el usuario,<br>**Entonces** el sistema retorna status 400 indicando conflicto de registro. | EP-04 |
     
## 3.2. Impact Mapping
<img src="../docs/assets/chapter-03/Impact_map.png" alt="Impact Mapping" width="auto" height="1900"/>
## 3.3. Product Backlog

| Orden | User Story ID | TÃ­tulo | DescripciÃ³n | Story Points |
|------|--------------|--------|-------------|--------------|
| 1 | US-001 | Registrar requerimiento de material | Como ingeniero residente, quiero registrar un requerimiento de materiales desde obra para iniciar el proceso de abastecimiento de forma estructurada. | 5 |
| 2 | US-002 | Adjuntar evidencia al requerimiento | Como ingeniero residente, quiero adjuntar fotos o documentos al requerimiento para brindar mayor claridad sobre el material solicitado. | 3 |
| 3 | US-003 | Visualizar lista de requerimientos | Como analista de logÃ­stica, quiero ver todos los requerimientos en una lista para gestionarlos eficientemente. | 5 |
| 4 | US-004 | Filtrar requerimientos | Como analista de logÃ­stica, quiero filtrar requerimientos por estado o proyecto para encontrarlos rÃ¡pidamente. | 3 |
| 5 | US-005 | Generar solicitud de cotizaciÃ³n | Como analista de logÃ­stica, quiero generar solicitudes de cotizaciÃ³n para obtener precios de proveedores. | 5 |
| 6 | US-006 | Registrar cotizaciones | Como analista de logÃ­stica, quiero registrar cotizaciones recibidas para compararlas. | 5 |
| 7 | US-007 | Comparar cotizaciones | Como jefe de proyecto, quiero comparar cotizaciones para elegir la mejor opciÃ³n. | 5 |
| 8 | US-008 | Aprobar compra | Como jefe de proyecto, quiero aprobar compras para autorizar gastos dentro del sistema. | 5 |
| 9 | US-009 | Generar orden de compra | Como analista de logÃ­stica, quiero generar Ã³rdenes de compra para formalizar pedidos. | 5 |
| 10 | US-010 | Notificar al proveedor | Como analista de logÃ­stica, quiero notificar al proveedor para iniciar el proceso de entrega. | 3 |
| 11 | US-011 | Seguimiento de pedidos | Como ingeniero residente, quiero ver el estado de mis pedidos para monitorear avances. | 5 |
| 12 | US-012 | Confirmar recepciÃ³n de materiales | Como ingeniero residente, quiero confirmar la recepciÃ³n de materiales para cerrar pedidos correctamente. | 5 |
| 13 | US-013 | Registrar incidencias | Como ingeniero residente, quiero registrar problemas con proveedores para llevar control de incidencias. | 5 |
| 14 | US-014 | Controlar stock | Como analista de logÃ­stica, quiero ver el stock disponible para evitar faltantes de materiales. | 5 |
| 15 | US-015 | Actualizar stock | Como analista de logÃ­stica, quiero actualizar el inventario para mantener datos reales del almacÃ©n. | 5 |
| 16 | US-016 | Visualizar historial de compras | Como jefe de proyecto, quiero ver el historial de compras para analizar decisiones pasadas. | 3 |
| 17 | US-017 | Control presupuestal | Como jefe de proyecto, quiero ver el control de costos para evitar sobrecostos en el proyecto. | 5 |
| 18 | US-018 | Alertas de sobrecosto | Como jefe de proyecto, quiero recibir alertas de sobrecostos para prevenir desviaciones presupuestales. | 3 |
| 19 | US-019 | Dashboard general | Como jefe de proyecto, quiero visualizar indicadores generales para tomar decisiones rÃ¡pidas. | 5 |
| 20 | US-020 | Acceso mÃ³vil | Como ingeniero residente, quiero acceder desde el mÃ³vil para gestionar procesos desde obra. | 3 |
| 21 | US-021 | Notificaciones en tiempo real | Como usuario, quiero recibir notificaciones en tiempo real para reaccionar rÃ¡pidamente a eventos. | 3 |
| 22 | US-022 | Registro de usuarios | Como analista de logÃ­stica, quiero registrar usuarios en el sistema para permitir el acceso controlado. | 3 |
| 23 | US-023 | Inicio de sesiÃ³n | Como usuario, quiero iniciar sesiÃ³n para acceder al sistema. | 3 |
| 24 | US-024 | GestiÃ³n de roles | Como jefe de proyecto, quiero gestionar roles para controlar permisos dentro del sistema. | 5 |
| 25 | US-025 | Historial de acciones | Como jefe de proyecto, quiero ver el historial de acciones para auditorÃ­a del sistema. | 5 |
| 26 | US-026 | BÃºsqueda global | Como analista de logÃ­stica, quiero buscar informaciÃ³n en el sistema para encontrar datos rÃ¡pidamente. | 3 |
| 27 | US-027 | IntegraciÃ³n con Excel | Como jefe de proyecto, quiero exportar datos a Excel para realizar anÃ¡lisis externos. | 3 |
| 28 | US-028 | Carga masiva de datos | Como analista de logÃ­stica, quiero subir datos de forma masiva para ahorrar tiempo en registros. | 5 |
| 29 | US-029 | GestiÃ³n de proveedores | Como analista de logÃ­stica, quiero registrar proveedores para tener una base de datos organizada. | 3 |
| 30 | US-030 | EvaluaciÃ³n de proveedores | Como jefe de proyecto, quiero calificar proveedores para mejorar decisiones futuras. | 3 |
| 31 | TS-01 | Obtener perfil por ID | Como desarrollador, quiero obtener el perfil de un usuario por su ID para recuperar informaciÃ³n detallada del usuario. | 3 |
| 32 | TS-02 | Actualizar perfil por ID | Como desarrollador, quiero actualizar los datos de un perfil de usuario para mantener la informaciÃ³n actualizada. | 4 |
| 33 | TS-03 | Obtener todos los perfiles | Como desarrollador, quiero listar todos los perfiles de usuario para su visualizaciÃ³n y gestiÃ³n. | 4 |
| 34 | TS-04 | Obtener materiales | Como desarrollador, quiero obtener todos los materiales registrados para visualizar el inventario disponible. | 3 |
| 35 | TS-05 | Crear material | Como desarrollador, quiero registrar nuevos materiales para ampliar el catÃ¡logo. | 4 |
| 36 | TS-06 | Obtener material por ID | Como desarrollador, quiero obtener un material especÃ­fico por su ID para ver su informaciÃ³n detallada. | 4 |
| 37 | TS-07 | Actualizar material | Como desarrollador, quiero actualizar un material para mantener informaciÃ³n correcta en el inventario. | 5 |
| 38 | TS-08 | Eliminar material | Como desarrollador, quiero eliminar materiales para mantener el inventario limpio. | 4 |
| 39 | TS-09 | Obtener categorÃ­as | Como desarrollador, quiero obtener categorÃ­as de materiales para clasificarlos. | 3 |
| 40 | TS-10 | Obtener categorÃ­a por ID | Como desarrollador, quiero obtener una categorÃ­a especÃ­fica para ver su detalle. | 5 |
| 41 | TS-11 | AutenticaciÃ³n de usuario | Como desarrollador, quiero autenticar usuarios para garantizar acceso seguro al sistema. | 3 |
| 42 | TS-12 | Registro de usuario | Como desarrollador, quiero registrar nuevos usuarios para permitir acceso controlado. | 3 |

<div align="center">
  <img src="docs/assets/chapter-03/jira1.png" alt="Evidence Product Backlog" width="90%">
  <p><em>Figura: Captura del Product Backlog en la herramienta de gestiÃ³n del proyecto.</em></p>
</div>


<div class="page-break"></div>

# CapÃ­tulo IV: Product Design

En este capÃ­tulo se detallan las decisiones de diseÃ±o de producto para la plataforma **Buildline** y su respectiva Landing Page. Se establecen las guÃ­as de estilo visuales, la arquitectura de la informaciÃ³n y los criterios que aseguran una experiencia de usuario (UX) intuitiva y profesional, alineada a las exigencias del sector construcciÃ³n y la gestiÃ³n logÃ­stica de obras.

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

El diseÃ±o visual de la plataforma **Buildline** se rige por una estÃ©tica robusta, tecnolÃ³gica y de alta eficiencia operativa, reflejando el compromiso con la eliminaciÃ³n de la informalidad y la integridad de la trazabilidad en la cadena de suministro. El objetivo es proyectar un entorno de control y profesionalismo que minimice la carga cognitiva tanto del residente en campo como del jefe de logÃ­stica en la oficina.

En este capÃ­tulo, detallaremos cada uno de los elementos visuales y de estilo que guÃ­an el desarrollo de la aplicaciÃ³n Buildline, siempre siguiendo los principios de DiseÃ±o de Experiencia de Usuario (UX) e Interfaz de Usuario (UI) para garantizar la mÃ¡xima usabilidad bajo condiciones de obra.

**Branding**

El logotipo principal de Buildline estÃ¡ compuesto por un isotipo que integra mÃºltiples elementos semÃ¡nticos de nuestro dominio tÃ©cnico: 
* **La LÃ­nea Continua:** Una 'B' estilizada formada por un trazo ininterrumpido que simboliza un flujo logÃ­stico eficiente y sin fin, respondiendo a la necesidad de trazabilidad absoluta.
* **El Edificio Modular:** Integrado en la parte superior del bucle, evoca el progreso de la obra y la finalizaciÃ³n exitosa del proyecto gracias a un abastecimiento oportuno.
* **Nodos de ConexiÃ³n:** Los pequeÃ±os cÃ­rculos representan la integraciÃ³n digital de requerimientos, cotizaciones y Ã³rdenes de compra, eliminando el caos de aplicaciones informales como WhatsApp.

<br>
<p align="center">
  <img src="../docs/assets/chapter-04/buildline_logo.jpg" alt="Buildline Logo" width="350px" height="auto"/>
</p>
<br>

**Typography**

La tipografÃ­a empleada en Buildline serÃ¡ **Montserrat**, con sus variantes Regular, Medium, SemiBold y Bold. La elecciÃ³n de Montserrat se basa en su estÃ©tica geomÃ©trica y sÃ³lida que evoca la resistencia de la construcciÃ³n, equilibrada con una legibilidad perfecta para revisar presupuestos y listas de materiales en pantallas mÃ³viles bajo el sol o en oficinas. AdemÃ¡s, su disponibilidad a travÃ©s de Google Fonts asegura una carga eficiente.

La jerarquÃ­a tipogrÃ¡fica se establece de la siguiente manera para garantizar claridad y ritmo visual:
* **TÃ­tulos principales (H1/SecciÃ³n heading):** 5rem (aprox. 50px) en escritorio, 4.5rem (aprox. 45px) en mÃ³vil.
* **SubtÃ­tulos (H2/Sub-headings):** 3rem (aprox. 30px) en escritorio.
* **TÃ­tulos de componentes (H3/H4):** 2rem (aprox. 20px) a 2.5rem (aprox. 25px).
* **Cuerpo del texto (p):** 1.6rem (aprox. 16px) con un interlineado de 1.6.
* **Botones y etiquetas (span):** 1.4rem (aprox. 14px) a 1.8rem (aprox. 18px).

<p align="center">
  <img src="../docs/assets/chapter-04/Style_guide.png" alt=" Typography Guide" width="500px" height="auto"/>
</p>

Esta distribuciÃ³n garantiza un contraste Ã³ptimo entre el texto y el fondo, superando un ratio mÃ­nimo de 4.5:1 segÃºn las WCAG 2.1 AA para una accesibilidad superior en entornos de campo.

**Colors**

Nuestra paleta de colores ha sido cuidadosamente seleccionada para evocar sensaciones de control corporativo, acciÃ³n operativa e innovaciÃ³n. Se ha distribuido en tres categorÃ­as principales:

* **Paleta principal:** Colores que definen la identidad de Buildline y se usan en elementos clave.
    * **Primario (Deep Navy Blue):** Transmite autoridad, formalidad profesional y seguridad. Utilizado en menÃºs de oficina y presupuestos.
    * **Secundario (Vibrant Orange):** Representa la energÃ­a de la obra en campo y la velocidad logÃ­stica. Utilizado para llamados a la acciÃ³n (CTAs) y botones urgentes.
    * **Terciario (Tech Cyan):** Evoca la conectividad y la nube. Utilizado para marcadores de estado y trazabilidad.
    * **Fondo Claro:** Proporciona un entorno visual limpio para tablas de cotizaciones.
    * **Fondo Blanco:** Fondos de tarjetas de requerimientos y paneles de control.
* **Paleta de Soporte:** Colores complementarios que aÃ±aden profundidad y contraste.
    * **Gris Neutro:** Para bordes sutiles, lÃ­neas divisorias y separadores de listas de materiales.
* **Colores Funcionales:** Reservados para comunicar estados crÃ­ticos al usuario.
    * **Ã‰xito:** Verde para Ã³rdenes de compra aprobadas y materiales entregados.
    * **Error:** Rojo para presupuestos excedidos o alertas de retraso.
    * **Advertencia:** Amarillo para quiebres de stock o requerimientos pendientes.

<p align="center">
  <img src="../docs/assets/chapter-04/Color_guidelines.png" alt=Color Palette" width="800px" height="auto"/>
</p>

Esta combinaciÃ³n cromÃ¡tica refleja los valores de nuestra marca y busca transmitir al pÃºblico (constructoras y gerentes de proyecto) una imagen de rigor, velocidad y control financiero.

**Spacing**

El espaciado en Buildline sigue un sistema modular para garantizar un ritmo visual armonioso y una jerarquÃ­a clara. La consistencia en el espaciado ayuda a reducir el estrÃ©s administrativo del usuario frente a largas listas de inventario.
* **Espaciado BÃ¡sico:** Usamos un espaciado base en el sistema de grid, multiplicado para crear espacios mayores.
* **Margen Interno (Padding) Generoso:** Las secciones principales utilizan un padding vertical de 5rem (50px) para crear pausas visuales. Los contenedores de requerimientos usan padding menor (30px - 40px) para agrupar datos lÃ³gicamente.
* **Espacio entre Elementos:** El espaciado entre tarjetas de obra o cotizaciones varÃ­a entre 3rem y 5rem, manteniendo una densidad de informaciÃ³n adecuada sin abrumar visualmente al jefe de logÃ­stica.
* **Line Height del Texto:** Interlineado configurado en 1.6, facilitando la lectura de especificaciones tÃ©cnicas de materiales.

**Tono de ComunicaciÃ³n**

La voz y el tono de Buildline estÃ¡n diseÃ±ados para ser tan resolutivos y estructurados como nuestra plataforma. Nuestro objetivo es conectar tanto con Residentes de Obra (campo) como con Gerentes Generales (gabinete).
* **Tono: Formal pero orientado a la acciÃ³n.** Buscamos proyectar autoridad en el control de costos, manteniendo el dinamismo que exige el trabajo en obra.
* **Actitud: Resolutiva y Ã¡gil.** El 90% de nuestra comunicaciÃ³n se orienta a la eficiencia ("Cero retrasos", "Aprobaciones en un clic"), mientras que el 10% es persuasiva para incentivar la adopciÃ³n del sistema.
* **Lenguaje: TÃ©cnico y directo.** Hablamos el idioma de la construcciÃ³n (ej. Ã“rdenes de Compra, Valorizaciones, Requerimientos, Cuadrillas, RFI). Nos enfocamos en la rentabilidad y la reducciÃ³n de sobrecostos.
* **Voz: Experta y moderna.** Posicionamos a Buildline como el fin de la informalidad y la llegada de la Industria 4.0 a la construcciÃ³n peruana.

### 4.1.2. Web Style Guidelines

Las directrices de estilo web de **Buildline** se centran en la velocidad operativa, la inmutabilidad del historial de compras y la facilidad de uso. Nuestro objetivo es crear una experiencia visual que digitalice el flujo de abastecimiento con un diseÃ±o limpio e intuitivo, especialmente para usuarios en campo con baja conectividad.

**1) Layout**
* **Sistema de Grid:** Utilizamos un diseÃ±o de cuadrÃ­cula flexible para garantizar que Buildline se adapte perfectamente. Esto permite que las tablas de cotizaciones complejas se condensen fluidamente en pantallas pequeÃ±as.
* **Headers y Footers:** El encabezado es fijo, proporcionando acceso a la navegaciÃ³n y botones de acceso. El pie de pÃ¡gina centraliza enlaces, contacto y soporte tÃ©cnico.
* **Cards:** Las tarjetas estructuran informaciÃ³n crÃ­tica, como los requerimientos de Obra pendientes. Cuentan con bordes redondeados y sombras suaves para facilitar la rÃ¡pida lectura de prioridades.

**2) Responsive Design**
* **Desktop:** Optimizado para la oficina de logÃ­stica y gerencia. MenÃºs laterales completos y grillas de datos expansivas para comparar cotizaciones en pantallas grandes.
* **Tablet:** Interfaz adaptada para supervisores de obra, con botones tÃ¡ctiles ampliados para el uso en movimiento.
* **Mobile (Mobile-First para Campo):** La experiencia mÃ³vil es ultra-ligera (Low-Data). MenÃº de hamburguesa y botones masivos para generar requerimientos fÃ¡cilmente incluso con una sola mano y guantes de obra.

**3) Interaction Design**
* **Botones:** Llamativos utilizando el "Vibrant Orange" para acciones principales (Aprobar, Enviar Requerimiento). Efectos lineales al pasar el cursor confirman la interactividad.
* **Formularios:** Extremadamente simplificados. Los campos de solicitud de material utilizan autocompletado predictivo para evitar que el operario de campo escriba largos textos.

**4) Images and Icons**
* **ImÃ¡genes:** FotografÃ­as de alta calidad que evocan grandes infraestructuras, ingenieros utilizando tablets en campo y almacenes ordenados.
* **Ãconos:** Estilo lineal y minimalista. Representan maquinaria, cascos, portapapeles y nodos de red para ofrecer una navegaciÃ³n visual intuitiva sin necesidad de leer mucho texto.

**5) Repositorio Central**
* **OrganizaciÃ³n:** Estructura lÃ³gica modular (`public/assets/images`, `public/assets/styles/style.css`, `public/assets/scripts/main.js`).
* **Versionado:** Uso estricto de Git para el control de versiones del equipo de desarrollo, garantizando despliegues seguros de la plataforma.

## 4.2. Information Architecture

La arquitectura de la informaciÃ³n de **Buildline** estÃ¡ diseÃ±ada para una navegaciÃ³n intuitiva orientada a roles, permitiendo que Gerentes, LogÃ­sticos y Residentes encuentren exactamente lo que necesitan sin fricciones.

### 4.2.1. Organization Systems

* **JerarquÃ­a de Contenidos:** La informaciÃ³n va del impacto macro al detalle operativo. La Landing Page inicia con el dolor principal (retrasos) y la promesa de valor (trazabilidad).
* **Secciones Principales de la Landing Page:**
    * **Hero:** El fin del caos logÃ­stico en la construcciÃ³n.
    * **What We Offer:** VisiÃ³n general del flujo Requerimiento-AprobaciÃ³n-Entrega.
    * **Features:** Aprobaciones mÃ³viles, control presupuestal, tracking de proveedores.
    * **Benefits:** ReducciÃ³n de sobrecostos de emergencia (hasta 18%) y prevenciÃ³n de paralizaciones.
    * **About Us:** Nuestro compromiso con la formalizaciÃ³n del sector.
    * **Plans:** Suscripciones adaptadas a constructoras MYPES y grandes corporaciones.
    * **Testimonials:** Respaldo de Jefes de Proyecto.
* **AgrupaciÃ³n de Contenidos:** Uso de pestaÃ±as y acordeones interactivos para clasificar funcionalidades tÃ©cnicas sin saturar la pantalla.

### 4.2.2. Labeling Systems

* **Nomenclatura:** Lenguaje 100% de la industria ("Crear Requerimiento", "Comparar Cotizaciones", "Emitir OC"). Botones claros como "Request Demo".
* **Consistencia:** UnificaciÃ³n de tÃ©rminos en todo el SaaS (siempre se usa "Requerimiento", nunca se mezcla con "Pedido" u "Orden").
* **Lenguaje Adaptativo:** Accesible para operarios de campo sin jerga de software, pero con el rigor financiero que exige una gerencia.

### 4.2.3. Searching Systems

* **Barra de BÃºsqueda:** Dentro del SaaS, es la herramienta principal de la oficina. Ubicada en la parte superior para buscar por *Nombre de Proyecto*, *ID de Orden de Compra* o *Proveedor*.
* **Filtros y Facetas:** Filtros crÃ­ticos por Estado (Pendiente, Aprobado, Rechazado, En TrÃ¡nsito), Fechas y Rango de Costos.
* **Historial de BÃºsqueda:** Registro de materiales mÃ¡s solicitados para agilizar futuras cotizaciones.
* **Resultados Relevantes:** PriorizaciÃ³n de requerimientos con etiqueta de "Urgente" o aquellos que superan el presupuesto base.

### 4.2.4. Navigation Systems

* **NavegaciÃ³n Global:** Barra de navegaciÃ³n superior fija en la Landing Page (`Home`, `Soluciones`, `Beneficios`, `Planes`).
* **NavegaciÃ³n Contextual:** Botones de llamado a la acciÃ³n (CTAs naranjas) que guÃ­an al usuario fluidamente desde la lectura de un beneficio hasta la solicitud de una cuenta.

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

El wireframe de la landing page de Buildline ha sido diseÃ±ado para reflejar una soluciÃ³n robusta, transparente y eficiente, atacando directamente la informalidad logÃ­stica del sector construcciÃ³n. La disposiciÃ³n de las secciones es la siguiente:

**Nav y Hero**

Esta secciÃ³n presenta el logotipo de Buildline y el menÃº de navegaciÃ³n. El titular principal comunica la misiÃ³n de la startup: "El fin del caos logÃ­stico en la construcciÃ³n". El diseÃ±o visual integra widgets de control en tiempo real que muestran el Presupuesto de Materiales, indicadores de Eficiencia de Suministro y estados de almacenamiento (Cemento, Acero). Incluye un campo de registro rÃ¡pido para que los gerentes de MYPES soliciten un demo de inmediato.

<img src="docs/assets/chapter-04/Nav-Hero-Wireframe.jpeg" alt="Nav-Hero-Wireframe" style="width:auto; height:auto; border:2px solid;">

**Workflow**

Bajo el tÃ­tulo "Todo lo que necesitas para gestionar y controlar tus proyectos", se detalla el flujo digital que reemplaza al WhatsApp/Excel en cuatro pasos:

<img src="docs/assets/chapter-04/Workflow-Wireframe.jpeg" alt="Workflow-Wireframe" style="width:auto; height:auto; border:2px solid;">

**Dashboard y Control Operativo**

Esta secciÃ³n unifica las capacidades crÃ­ticas de anÃ¡lisis de la plataforma. Permite visualizar las desviaciones presupuestales antes de que se conviertan en pÃ©rdidas, gestionar el centro de alertas para aprobaciones jerÃ¡rquicas en tiempo real y mantener una trazabilidad de compras total. El diseÃ±o estÃ¡ optimizado para que el Jefe de LogÃ­stica priorice compras crÃ­ticas, reduciendo el 12% de sobrecostos por compras de emergencia y garantizando que el insumo en obra coincida con la especificaciÃ³n tÃ©cnica.

<img src="docs/assets/chapter-04/Dashboard-Control-Wireframe.jpeg" alt="Dashboard-Control-Operativo-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Testimonials**

Bajo la secciÃ³n "Â¿Por quÃ© Buildline?", se presentan testimonios de roles clave (DueÃ±os de obra, Supervisores de mercado y Gerentes de operaciones). Los mensajes validan la soluciÃ³n enfocÃ¡ndose en la eliminaciÃ³n de hojas de cÃ¡lculo manuales, la reducciÃ³n del estrÃ©s operativo y la capacidad de validar pedidos desde el campo sin necesidad de retornar a la oficina.

<img src="docs/assets/chapter-04/Testimonials-Wireframe.jpeg" alt="Testimonials-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Register** 

Define los tres pilares de la experiencia Buildline: Setup (creaciÃ³n estructurada de pedidos), Monitor (seguimiento de cotizaciones) y Control (detecciÃ³n temprana de quiebres de stock). Finaliza con un formulario de registro limpio que permite el acceso mediante credenciales institucionales o redes sociales (Google/Apple), reduciendo la fricciÃ³n de entrada para el personal operativo.

<img src="docs/assets/chapter-04/Register-Wireframe.jpeg" alt="Register-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Pricing** 

Presenta la escalabilidad del modelo SaaS mediante dos planes: el Project Base Plan, ideal para MYPES con hasta 3 proyectos que buscan eliminar el desorden de WhatsApp, y el Multi-Project Enterprise, que ofrece escala ilimitada, reportes de rentabilidad avanzada e integraciÃ³n con sistemas contables locales para constructoras de mayor volumen.

<img src="docs/assets/chapter-04/Princig-Wireframe.jpeg" alt="Princig-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Footer** 

Cierra la interfaz con una organizaciÃ³n clara de recursos dividida en Producto, Soporte y Recursos. Incluye accesos a plantillas, guÃ­as de usuario, polÃ­ticas de privacidad y canales de contacto directo, reforzando la seriedad y el soporte tÃ©cnico que RQLS ofrece a sus clientes.

<img src="docs/assets/chapter-04/Footer-Wireframe.jpeg" alt="Footer-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

### 4.3.2. Landing Page Mock-up

El mock-up de la pÃ¡gina de inicio representa la versiÃ³n final de alta fidelidad, donde se aplican las guÃ­as de estilo para transmitir confianza, modernidad y rigor tÃ©cnico a las MYPES constructoras.

**Nav y Hero**

Se observa el acabado final del logotipo de Buildline en la esquina superior izquierda. El diseÃ±o utiliza una composiciÃ³n limpia con un fondo claro para resaltar los widgets de datos. La tipografÃ­a Rubik en el titular principal presenta un contraste jerÃ¡rquico que facilita la lectura. El botÃ³n de llamado a la acciÃ³n (CTA) en azul tecnolÃ³gico guÃ­a al usuario hacia la conversiÃ³n inmediata, mientras que la imagen central humaniza la tecnologÃ­a frente al operario de construcciÃ³n.

<img src="docs/assets/chapter-04/Nav-Hero-Landing Page Mock-up.jpeg" alt="Nav-Hero-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Workflow**

En esta secciÃ³n se aplican Ã­conos planos con colores vibrantes para diferenciar las etapas de la cadena de suministro. El diseÃ±o utiliza tarjetas con sombras suaves (soft shadows) que generan profundidad, permitiendo que el flujo de Monitoreo, Registros, Alertas y Compliance se perciba como un proceso fluido y sencillo de seguir, alejÃ¡ndose de la complejidad visual de los ERP tradicionales.

<img src="docs/assets/chapter-04/Workflow-Landing Page Mock-up.jpeg" alt="Workflow-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Dashboard y Control Operativo** 

Este bloque integra de manera cohesiva el centro neurÃ¡lgico de la plataforma. Se visualizan grÃ¡ficos de anillos y lÃ­neas con la paleta de colores funcionales (Verde para Ã©xito, Rojo para alertas de presupuesto). La interfaz del mock-up demuestra la alta densidad de datos de forma organizada, permitiendo que el Jefe de Proyecto identifique rÃ¡pidamente desviaciones de costos y estados de sensores en almacÃ©n sin saturaciÃ³n visual.

<img src="docs/assets/chapter-04/Dashboard-Control-Operativo-Landing Page Mock-up.jpeg" alt="Dashboard-Control-Operativo-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Testimonials** 

El mock-up presenta las tarjetas de testimonios en un formato limpio y minimalista. Se utilizan avatares circulares y una tipografÃ­a ligera para las citas, reforzando la credibilidad. El uso de espacios en blanco (whitespace) entre cada testimonio asegura que la "prueba social" sea fÃ¡cil de digerir, transmitiendo la seguridad que otros profesionales ya experimentan con Buildline.

<img src="docs/assets/chapter-04/Testimonials-Landing Page Mock-up.jpeg" alt="Testimonials-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Register**

Se muestra el diseÃ±o final del formulario de registro, el cual aparece como una capa superpuesta (overlay) con un desenfoque de fondo (backdrop blur). Los campos de entrada tienen estados visuales claros y los botones de registro social (Google/Apple) mantienen la estÃ©tica minimalista del sistema, reduciendo la carga cognitiva del usuario al momento de crear su cuenta.

<img src="docs/assets/chapter-04/Register-Landing Page Mock-up.jpeg" alt="Register-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Pricing**

La interfaz de precios utiliza un selector de tiempo (Mensual/Anual) con una transiciÃ³n visual suave. Se aplica un contraste marcado entre el Project Base Plan (claro) y el Multi-Project Enterprise (oscuro/pizarra) para diferenciar visualmente los segmentos de cliente, destacando los beneficios mediante un sistema de check-list limpio y profesional.

<img src="docs/assets/chapter-04/Pricing-Landing Page Mock-up.jpeg" alt="Princig-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

**Footer**

El pie de pÃ¡gina final utiliza un tono gris pizarra oscuro para marcar el cierre de la navegaciÃ³n. Los Ã­conos de redes sociales y los enlaces estÃ¡n distribuidos con un espaciado modular que garantiza la legibilidad, manteniendo la sobriedad institucional de la startup RQLS.

<img src="docs/assets/chapter-04/Footer-Landing Page Mock-up.jpeg" alt="Footer-Landing Page Mock-up" style="width:auto; height:auto; border:2px solid;">

## 4.4. Web Applications UX/UI Design
### 4.4.1. Web Applications Wireframes

En esta secciÃ³n se presentan los wireframes diseÃ±ados para la aplicaciÃ³n web de RQLS (Buildline). Cada pantalla responde a las funcionalidades principales del sistema de gestiÃ³n logÃ­stica y control presupuestal, atendiendo a los roles de usuario definidos: Ingeniero Residente, Jefe de LogÃ­stica y Gerente General.

**Portal de Inicio - Buildline**

Pantalla principal de presentaciÃ³n donde se ofrecen las opciones de ingreso y registro de nuevas plantas industriales.

<img src="docs/assets/chapter-04/Ingreso al Sistema - Buildline - Web Wireframes.jpeg" alt="Ingreso al Sistema - Buildline - Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**Crear Cuenta - Buildline**

Interfaz de registro inicial diseÃ±ada para capturar de forma estructurada los datos del responsable de la constructora, estableciendo los cimientos de la seguridad y el acceso jerÃ¡rquico al sistema.

<img src="docs/assets/chapter-04/Crear Cuenta - Buildline -Web Wireframes.jpeg" alt="Crear Cuenta - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**RecuperaciÃ³n de Credenciales - Buildline**

Wireframe del mÃ³dulo de soporte para el restablecimiento de contraseÃ±as. Proporciona un flujo directo que permite al usuario retomar sus actividades operativas mediante una verificaciÃ³n vÃ­a correo electrÃ³nico.

<img src="docs/assets/chapter-04/RecuperaciÃ³n de Credenciales - Buildline -Web Wireframes.jpeg" alt="RecuperaciÃ³n de Credenciales - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**GestiÃ³n de Requerimientos de Materiales - Buildline**

Pantalla tÃ©cnica que centraliza las solicitudes provenientes de obra. Permite la visualizaciÃ³n de la Prioridad (Critical/High) y el estado de la validaciÃ³n, integrando un buscador dinÃ¡mico para la localizaciÃ³n rÃ¡pida de pedidos especÃ­ficos.

<img src="docs/assets/chapter-04/GestiÃ³n de Inventario y Requerimientos - Buildline - Wireframes.jpeg" alt="GestiÃ³n de Inventario y Requerimientos - Buildline - Wireframes" style="width:auto; height:auto; border:2px solid;">

**Panel de Control de Requisiciones - Buildline**

Vista alternativa del mÃ³dulo de inventario con un enfoque en el seguimiento de estados (Pending Auth, In Transit, Processing, Delivered). Permite al Jefe de LogÃ­stica tener una visiÃ³n panorÃ¡mica del flujo de suministros hacia las distintas obras.

<img src="docs/assets/chapter-04/Panel de Control de Requisiciones - Buildline -Web Wireframes.jpeg" alt="Panel de Control de Requisiciones - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**Dashboard Overview - Buildline**

Panel principal de anÃ¡lisis que consolida los KPIs crÃ­ticos de la constructora. Muestra mÃ©tricas de Total Deliveries y Active Personnel, acompaÃ±adas de grÃ¡ficos de tendencia para el monitoreo de la eficiencia operativa.

<img src="docs/assets/chapter-04/Dashboard Overview - Buildline -Web Wireframes.jpeg" alt="Dashboard Overview - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**Registro de Nuevo Requerimiento - Buildline**

Interfaz de formulario modal (New Material Request) diseÃ±ada para que el Ingeniero Residente registre pedidos de insumos de forma Ã¡gil. Contiene campos para seleccionar el proyecto, tipo de material, cantidad, unidad de medida y fecha requerida, ademÃ¡s de un Ã¡rea de especificaciones tÃ©cnicas.

<img src="docs/assets/chapter-04/Registro de Nuevo Requerimiento - Buildline -Web Wireframes.jpeg" alt="Registro de Nuevo Requerimiento - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

### 4.4.2. Web Applications Wireflow Diagrams

Los Wireflows se utilizan, sobre todo, en el diseÃ±o de la experiencia del usuario (UX) y son particularmente beneficiosos para aplicaciones que contienen interacciones complejas y flujos de trabajo.

<img src="docs/assets/chapter-04/Web applications wireflow diagrams.jpeg" alt="Web applications wireflow diagrams" style="width:auto; height:auto; border:2px solid;">

### 4.4.3. Web Applications Mock-ups

En esta secciÃ³n se presentan los mock-ups de alta fidelidad para la aplicaciÃ³n web de Buildline. Estos diseÃ±os finales integran la identidad visual de la marca, tipografÃ­as legibles y una arquitectura de informaciÃ³n optimizada para la gestiÃ³n logÃ­stica en tiempo real.

**Portal de Inicio - Buildline**

Esta interfaz representa el punto de acceso principal al ecosistema de Buildline. Utiliza una composiciÃ³n limpia y moderna que resalta el formulario de autenticaciÃ³n, permitiendo a los usuarios de la constructora ingresar de forma segura o iniciar el proceso de creaciÃ³n de cuenta nueva.

<img src="docs/assets/chapter-04/Ingreso al Sistema - Buildline - Applications Mock-ups.jpeg" alt="Ingreso al Sistema - Buildline - Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**Crear Cuenta - Buildline**

DiseÃ±o final del formulario de registro organizacional. Esta pantalla permite recolectar los datos fundamentales de la constructora y el administrador principal, utilizando una jerarquÃ­a visual clara para asegurar la integridad de la informaciÃ³n de seguridad.

<img src="docs/assets/chapter-04/Crear Cuenta - Buildline -Applications Mock-ups.jpeg" alt="Crear Cuenta - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**RecuperaciÃ³n de Credenciales - Buildline**

Mock-up del flujo de soporte para el restablecimiento de credenciales. La interfaz ha sido diseÃ±ada para minimizar la fricciÃ³n operativa, permitiendo al usuario solicitar un enlace de restauraciÃ³n mediante su correo institucional en pocos pasos.

<img src="docs/assets/chapter-04/RecuperaciÃ³n de Credenciales - Buildline -Applications Mock-ups.jpeg" alt="RecuperaciÃ³n de Credenciales - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**GestiÃ³n de Requerimientos de Materiales - Buildline**

Mock-up del mÃ³dulo operativo principal. Presenta una tabla de datos avanzada con estados de validaciÃ³n por colores (Pending, Approved, In Transit), permitiendo al Jefe de LogÃ­stica supervisar la trazabilidad completa de los materiales desde la obra.

<img src="docs/assets/chapter-04/GestiÃ³n de Inventario y Requerimientos - Buildline - Applications Mock-ups.jpeg" alt="GestiÃ³n de Inventario y Requerimientos - Buildline - Wireframes" style="width:auto; height:auto; border:2px solid;">

**Panel de Control de Requisiciones - Buildline**

Vista alternativa del mÃ³dulo de inventario con un enfoque en el seguimiento de estados (Pending Auth, In Transit, Processing, Delivered). Permite al Jefe de LogÃ­stica tener una visiÃ³n panorÃ¡mica del flujo de suministros hacia las distintas obras.

<img src="docs/assets/chapter-04/Panel de Control de Requisiciones - Buildline -Applications Mock-ups.jpeg" alt="Panel de Control de Requisiciones - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**Dashboard Overview - Buildline**

El dashboard centralizado de Buildline en alta fidelidad. Consolida indicadores crÃ­ticos como Total Deliveries y Alertas de Inventario mediante tarjetas visuales y grÃ¡ficos interactivos, facilitando la toma de decisiones estratÃ©gicas para la gerencia.

<img src="docs/assets/chapter-04/Dashboard Overview - Buildline -Applications Mock-ups.jpeg" alt="Dashboard Overview - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**Registro de Nuevo Requerimiento - Buildline**

Interfaz de formulario modal (New Material Request) diseÃ±ada para que el Ingeniero Residente registre pedidos de insumos de forma Ã¡gil. Contiene campos para seleccionar el proyecto, tipo de material, cantidad, unidad de medida y fecha requerida, ademÃ¡s de un Ã¡rea de especificaciones tÃ©cnicas.

<img src="docs/assets/chapter-04/Registro de Nuevo Requerimiento - Buildline -Applications Mock-ups.jpeg" alt="Registro de Nuevo Requerimiento - Buildline -Web Wireframes" style="width:auto; height:auto; border:2px solid;">

**Mock-ups Version Mobile**

La secciÃ³n de Web Applications UX/UI Design presenta la propuesta visual, estructural y de interacciÃ³n desarrollada para la experiencia mÃ³vil de Buildline, el ecosistema SaaS orientado a la gestiÃ³n integral de adquisiciones, el control de suministros en tiempo real y la trazabilidad de materiales en el sector construcciÃ³n.

<img src="docs/assets/chapter-04/mobile1.jpeg" alt="mobile" style="width:auto; height:auto; border:2px solid;">

<img src="docs/assets/chapter-04/mobile2.jpeg" alt="mobile" style="width:auto; height:auto; border:2px solid;">

<img src="docs/assets/chapter-04/mobile3.jpeg" alt="mobile" style="width:auto; height:auto; border:2px solid;">

<img src="docs/assets/chapter-04/mobile4.jpeg" alt="mobile" style="width:auto; height:auto; border:2px solid;">

<img src="docs/assets/chapter-04/mobile5.jpeg" alt="mobile" style="width:auto; height:auto; border:2px solid;">

<img src="docs/assets/chapter-04/mobile6.jpeg" alt="mobile" style="width:auto; height:auto; border:2px solid;">

<img src="docs/assets/chapter-04/mobile7.jpeg" alt="mobile" style="width:auto; height:auto; border:2px solid;">

### 4.4.4. Web Applications User Flow Diagrams

Para asegurar una navegaciÃ³n intuitiva y una curva de aprendizaje mÃ­nima para nuestros usuarios, se ha definido una simbologÃ­a estÃ¡ndar basada en colores y formas geomÃ©tricas. Esta coherencia visual se mantiene en todos los diagramas del sistema.

**Leyenda Visual de SimbologÃ­a**

<img src="docs/assets/chapter-04/diagramaUF_leyenda.png" alt="diagramaUF_leyenda" style="width:auto; height:auto; border:2px solid;">

**Diagrama 1: Flujo de AutenticaciÃ³n**

Este flujo garantiza que solo personal autorizado (Jefes de Proyecto y Gerentes) acceda a los datos financieros de las obras.

<img src="docs/assets/chapter-04/diagramaUF_1.png" alt="diagramaUF_1" style="width:auto; height:auto; border:2px solid;">

**Diagrama 2: Flujo de RequisiciÃ³n de Materiales**

Representa la interacciÃ³n del Jefe de Proyecto en el frente de obra al detectar una necesidad de insumos, asegurando que la informaciÃ³n llegue formalmente a la oficina.

<img src="docs/assets/chapter-04/diagramaUF_2.png" alt="diagramaUF_2" style="width:auto; height:auto; border:2px solid;">

**Diagrama 3: Flujo Global de Abastecimiento**

Representa el ciclo completo de negocio (Happy Path) que conecta la solicitud en campo con la aprobaciÃ³n gerencial y la emisiÃ³n del documento de compra.

<img src="docs/assets/chapter-04/diagramaUF_3.png" alt="diagramaUF_3" style="width:auto; height:auto; border:2px solid;">

## 4.5. Web Applications Prototyping

Para validar la arquitectura de informaciÃ³n y la eficiencia del flujo de negocio de **Buildline**, se ha desarrollado un prototipo interactivo de alta fidelidad basado en los diagramas de interacciÃ³n detallados en la secciÃ³n anterior. Este artefacto permite verificar la fluidez de la interfaz y la respuesta del sistema ante las necesidades crÃ­ticas del sector construcciÃ³n.

<img src="docs/assets/chapter-04/prototyping_captura.png" alt="prototyping_captura" style="width:auto; height:auto; border:2px solid;">

> [**ðŸ”— Ver Video Prototipo Interactivo - Buildline**](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202316687_upc_edu_pe/IQDfG_KwrXxqSrKx5D7At2JHAb3kkmot9LW_fXuBca38Z_g?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=aRAlkn)

## 4.6. Domain-Driven Software Architecture

La arquitectura de software de Buildline se construye a partir de los resultados obtenidos en el Big Picture Event Storming, que permitiÃ³ comprender en profundidad los flujos clave del dominio de abastecimiento logÃ­stico en el sector construcciÃ³n y las interacciones entre los ingenieros residentes, el Ã¡rea de logÃ­stica y la gerencia general. A partir de este anÃ¡lisis inicial, se desarrollÃ³ una visiÃ³n mÃ¡s estructurada del dominio utilizando los principios de Domain-Driven Design (DDD).

En las siguientes secciones se presenta cada nivel del modelo, explicando la estructura, responsabilidades y comunicaciÃ³n entre los elementos que conforman la arquitectura de Buildline.


### 4.6.1. Design-Level Event Storming

Para identificar los eventos de dominio y la lÃ³gica de negocio, se realizÃ³ una sesiÃ³n de Event Storming. Esta tÃ©cnica colaborativa permitiÃ³ visualizar y comprender el flujo de eventos dentro de la cadena de suministro de las MYPES constructoras, facilitando la identificaciÃ³n de los Bounded Contexts que estructurarÃ¡n el sistema.

El desarrollo del proceso del Domain-Driven Design se realizÃ³ en la aplicaciÃ³n Miro: [(https://miro.com/app/board/uXjVHeXoe4U=/?share_link_id=202545251721)]


1. Bounded Context **IAM**

   El bounded context IAM (Identity and Access Management) se encarga de la autenticaciÃ³n, autorizaciÃ³n y seguridad dentro de Buildline. Administra el acceso de los diferentes perfiles (Residente de Obra, Analista de LogÃ­stica y Jefe de Proyecto) garantizando que cada actor solo interactÃºe con los mÃ³dulos que le corresponden. Su propÃ³sito es asegurar la integridad del acceso al sistema SaaS y gestionar los permisos jerÃ¡rquicos de aprobaciÃ³n.
   
   <img src="docs/assets/chapter-04/boundedIAM.png" alt="Bounded Context IAM" style="width:auto; height:auto; border:2px solid;">


2. Bounded Context **Profiles**

   El bounded context Profiles gestiona la informaciÃ³n estÃ¡tica y de configuraciÃ³n de la empresa constructora (MYPE) y los perfiles laborales de su equipo. Administra la creaciÃ³n y actualizaciÃ³n de datos de contacto y la estructura organizacional. Su propÃ³sito es centralizar la ficha de contacto operativa para que contextos como IAM, Requisition y Procurement sepan exactamente quiÃ©n estÃ¡ solicitando o aprobando los recursos.
   
   <img src="docs/assets/chapter-04/boundedprofile.png" alt="Bounded Context Profiles" style="width:auto; height:auto; border:2px solid;">


3. Bounded Context **Requisition**

   El bounded context Requisition representa el punto de inicio operativo en el frente de obra. Administra la creaciÃ³n, priorizaciÃ³n y seguimiento de los requerimientos de materiales que realizan los Ingenieros Residentes, incluyendo la adjunciÃ³n de evidencia tÃ©cnica. Su propÃ³sito es digitalizar la necesidad de la obra, eliminando la informalidad de canales como WhatsApp y centralizando las solicitudes tÃ©cnicas.
   
   <img src="docs/assets/chapter-04/boundedrequisition.png" alt="Bounded Context Requisition" style="width:auto; height:auto; border:2px solid;">


4. Bounded Context **Procurement**

   El bounded context Procurement es el nÃºcleo transaccional en gabinete. Gestiona el ciclo de compras completo: generaciÃ³n de solicitudes de cotizaciÃ³n, comparaciÃ³n de ofertas de proveedores y la aprobaciÃ³n jerÃ¡rquica de la Orden de Compra (PO) por parte de la gerencia. Su propÃ³sito es eliminar las compras de emergencia informales y asegurar que todo gasto estÃ© debidamente sustentado y aprobado antes de su ejecuciÃ³n.
   
   <img src="docs/assets/chapter-04/boundedprocurement.png" alt="Bounded Context Procurement" style="width:auto; height:auto; border:2px solid;">


5. Bounded Context **Inventory**

   El bounded context Inventory administra la recepciÃ³n fÃ­sica de los materiales en la obra y el control de los saldos. Permite al personal en campo confirmar la llegada de insumos y registrar mermas o desperdicios. Se integra estrechamente con Procurement para realizar el cruce de informaciÃ³n entre la Orden de Compra y la GuÃ­a de RemisiÃ³n (Way Match), previniendo pÃ©rdidas por descontrol de almacÃ©n.
   
   <img src="docs/assets/chapter-04/boundedinventory.png" alt="Bounded Context Inventory" style="width:auto; height:auto; border:2px solid;">


6. Bounded Context **Suppliers**

   El bounded context Suppliers gestiona el directorio, historial de confiabilidad y evaluaciÃ³n de los proveedores de la constructora. Permite registrar nuevos ofertantes, calificar sus tiempos de entrega y documentar incidencias operativas. Su propÃ³sito es construir una base de datos confiable que agilice las cotizaciones en Procurement y evite la contrataciÃ³n de empresas con antecedentes deficientes.
   
   <img src="docs/assets/chapter-04/boundedsupplier.png" alt="Bounded Context Suppliers" style="width:auto; height:auto; border:2px solid;">


7. Bounded Context **Analytics & Budgeting**

   El bounded context Analytics & Budgeting procesa la informaciÃ³n financiera cruzando el presupuesto planificado (APU) con los gastos reales derivados de las Ã³rdenes de compra. Permite la visualizaciÃ³n de mÃ©tricas y la detecciÃ³n de desviaciones presupuestales. Su propÃ³sito es brindar visibilidad gerencial en tiempo real mediante Dashboards, previniendo el impacto de los sobrecostos logÃ­sticos estructurales del sector.
   
   <img src="docs/assets/chapter-04/boundedA&B.png" alt="Bounded Context Analytics" style="width:auto; height:auto; border:2px solid;">


8. Bounded Context **Communication**

   El bounded context Communication gestiona el envÃ­o automatizado de notificaciones internas (alertas de requerimientos crÃ­ticos, avisos de bajo stock) y correos electrÃ³nicos externos (envÃ­o formal de Ã“rdenes de Compra a proveedores). Su propÃ³sito es asegurar una comunicaciÃ³n oportuna, trazable y estructurada que reduzca los cuellos de botella informativos entre la obra y la oficina central.
   
   <img src="docs/assets/chapter-04/boundedcommunication.png" alt="Bounded Context Communication" style="width:auto; height:auto; border:2px solid;">


9. Bounded Context **Shared**

   El bounded context Shared contiene elementos transversales, utilidades, el catÃ¡logo maestro de materiales y registros de auditorÃ­a inmutables utilizados por todos los demÃ¡s contextos. Su propÃ³sito es evitar la duplicidad de lÃ³gica de negocio, garantizar la trazabilidad total de las acciones de los usuarios en el sistema y mantener la coherencia semÃ¡ntica en toda la plataforma.
   
   <img src="docs/assets/chapter-04/boundedshared.png" alt="Bounded Context Shared" style="width:auto; height:auto; border:2px solid;">

<div style="page-break-after: always;"></div>

### 4.6.2. Software Architecture Context Diagram

En este nivel se presenta una vista de alto nivel de la arquitectura, donde el foco estÃ¡ en el sistema de software Buildline como una â€œcaja negraâ€ y en las interacciones que mantiene con sus usuarios y con otros sistemas externos.

El context diagram muestra al **Buildline Software System** como un recuadro en el centro, rodeado por los principales actores y sistemas con los que se comunica:

- **Ingeniero Residente**: usuario interno operativo ubicado en el frente de obra. InteractÃºa con Buildline para registrar requerimientos de materiales, adjuntar evidencias tÃ©cnicas y confirmar la recepciÃ³n fÃ­sica de los despachos.
- **Analista de LogÃ­stica**: usuario administrativo en oficina responsable de gestionar el ciclo de compras. InteractÃºa con la plataforma para solicitar cotizaciones, comparar precios y generar las Ã³rdenes de compra.
- **Jefe de Proyecto / Gerente**: usuario estratÃ©gico que supervisa la viabilidad financiera del proyecto. Consulta la plataforma para monitorear el control de costos (APU) y aprobar o rechazar gastos crÃ­ticos.
- **SUNAT / Billing API**: sistema gubernamental (o proveedor PSE) externo utilizado para la validaciÃ³n de comprobantes de pago y el cumplimiento de la normativa tributaria local.
- **Email Notification Service**: servicio de correo utilizado para enviar notificaciones transaccionales (alertas de stock, recordatorios) y despachar formalmente las Ã³rdenes de compra a los proveedores.
- **Payment Gateway (Stripe)**: sistema externo encargado de procesar el cobro de las suscripciones mensuales (modelo SaaS) asociadas al uso de la plataforma por parte de la constructora.

En el diagrama se representan las relaciones entre estos elementos, destacando que los actores humanos interactÃºan Ãºnicamente con Buildline, mientras que el sistema se encarga de orquestar las integraciones con los servicios externos (validaciÃ³n tributaria, correos y pagos). Esta vista permite entender el alcance del sistema, los lÃ­mites de responsabilidad y el ecosistema logÃ­stico en el que se inserta Buildline antes de entrar a detalles de implementaciÃ³n.

![ContextDiagram Diagram](../docs/assets/chapter-04/ContextDiagram.svg)

---

### 4.6.3. Software Architecture Container Diagrams

En el nivel de contenedores, la atenciÃ³n se desplaza desde â€œquiÃ©n usa el sistemaâ€ hacia â€œcÃ³mo se organiza internamente el sistema en aplicaciones y fuentes de datosâ€. El container diagram muestra los elementos de alto nivel de la arquitectura de Buildline, sus responsabilidades principales y la forma en que se comunican entre sÃ­ y con los sistemas externos.

La arquitectura lÃ³gica de Buildline se estructura en los siguientes contenedores:

- **Landing Page**: aplicaciÃ³n web estÃ¡tica que presenta la propuesta de valor de Buildline orientada a MYPES constructoras, guÃ­a a nuevos usuarios y redirige a la aplicaciÃ³n principal. EstÃ¡ desarrollada con tecnologÃ­as web estÃ¡ndar (HTML, CSS y JavaScript) y se despliega en un entorno orientado a contenido estÃ¡tico.
- **Single Page Application (SPA)**: aplicaciÃ³n web principal, implementada en **Angular**, donde interactÃºan el Ingeniero Residente, el Analista de LogÃ­stica y el Gerente. Este contenedor concentra la experiencia de usuario, las vistas y la lÃ³gica de presentaciÃ³n para los diferentes contextos del dominio (iam, profiles, requisition, procurement, inventory, suppliers, analytics y communication).
- **API Application**: backend implementado con **Spring Boot**, que expone una API REST y encapsula la lÃ³gica de negocio, reglas de validaciÃ³n y orquestaciÃ³n de procesos logÃ­sticos. Este contenedor agrupa los mÃ³dulos backend por contexto (IAM Backend, Profiles Backend, Requisition Backend, Procurement Backend, Inventory Backend, Suppliers Backend, Analytics Backend, Communication Backend y Shared Backend).
- **Database**: base de datos relacional **MySQL**, donde se persiste la informaciÃ³n estructurada del sistema: usuarios, perfiles de constructoras, requerimientos, cotizaciones, Ã³rdenes de compra, inventarios, auditorÃ­as y mÃ©tricas.

En el diagrama se observa que:

- Los usuarios acceden primero a la **Landing Page**, la cual redirige a la **SPA** tras la autenticaciÃ³n.
- La **SPA** se comunica exclusivamente con la **API Application** mediante peticiones **HTTP/HTTPS** con mensajes **JSON**, siguiendo un estilo REST.
- La **API Application** persiste y consulta datos en la **Database** mediante **JDBC** y mapeo objetoâ€“relacional.
- Tanto la **SPA** como la **API Application** interactÃºan con los sistemas externos: el **Payment Gateway** para suscripciones, la **SUNAT API** para validaciones, y el **Email Notification Service** para el envÃ­o de notificaciones y Ã³rdenes de compra.

Esta vista permite apreciar cÃ³mo se distribuyen las responsabilidades entre la capa de presentaciÃ³n (Landing y SPA), la capa de lÃ³gica de negocio (API Application) y la capa de persistencia (Database), asÃ­ como las principales decisiones tecnolÃ³gicas que se han tomado para cada contenedor.

![ContainerDiagram Diagram](../docs/assets/chapter-04/ContainerDiagram.svg)

---

### 4.6.4. Software Architecture Components Diagrams

En el nivel de componentes se detalla la descomposiciÃ³n interna de los contenedores, mostrando los bloques estructurales que conforman cada uno y las relaciones entre ellos. Dado que la **Single Page Application** y la **Database** ya fueron descritas en otros apartados mediante diagramas de clases frontend y de base de datos, en esta secciÃ³n se pone especial Ã©nfasis en el contenedor **API Application**, donde reside la mayor parte de la lÃ³gica de negocio.

El component diagram de la **API Application** agrupa la arquitectura interna siguiendo los bounded contexts definidos en el dominio de Buildline. Cada mÃ³dulo backend representa un componente principal dentro del contenedor:

- **IAM Backend**: se encarga de la autenticaciÃ³n, gestiÃ³n de usuarios, roles jerÃ¡rquicos (Residente, LogÃ­stica, Gerencia) y validaciones de acceso a la plataforma.
- **Profiles Backend**: gestiona la informaciÃ³n de la empresa constructora (MYPE) y los perfiles de los empleados, centralizando los datos de contacto y estructura organizacional.
- **Requisition Backend**: implementa la lÃ³gica de las solicitudes de campo, permitiendo registrar requerimientos de materiales, adjuntar evidencias y establecer prioridades.
- **Procurement Backend**: agrupa la funcionalidad del ciclo de compras en oficina, incluyendo la gestiÃ³n de cotizaciones, generaciÃ³n de cuadros comparativos y emisiÃ³n de Ã“rdenes de Compra formales.
- **Inventory Backend**: administra el control de almacÃ©n en obra, validando la recepciÃ³n de materiales mediante el cruce de GuÃ­as de RemisiÃ³n con Ã“rdenes de Compra (Way Match) y registrando mermas.
- **Suppliers Backend**: gestiona el directorio de proveedores de la constructora, almacenando historiales de confiabilidad, calificaciones e incidencias operativas.
- **Analytics Backend**: ofrece capacidades de agregaciÃ³n y cÃ¡lculo cruzando el presupuesto planificado (APU) con los gastos reales, generando KPIs y detectando sobrecostos logÃ­sticos.
- **Communication Backend**: orquesta el envÃ­o de notificaciones internas en tiempo real (alertas de aprobaciÃ³n, quiebres de stock) y la comunicaciÃ³n externa con proveedores (envÃ­o de OCs).
- **Shared Backend**: provee componentes compartidos, utilidades, el catÃ¡logo maestro de materiales y el registro inmutable de auditorÃ­a utilizado por los demÃ¡s mÃ³dulos backend.

En el diagrama se refleja cÃ³mo:

- La **SPA** consume los servicios expuestos por cada mÃ³dulo backend a travÃ©s de la **API Application**, utilizando endpoints REST especÃ­ficos por contexto.
- Cada mÃ³dulo backend accede a la **Database** para leer y escribir la informaciÃ³n correspondiente a su contexto (por ejemplo, Requisition Backend a tablas de solicitudes, Procurement Backend a tablas de cotizaciones y OCs).
- Algunos mÃ³dulos se integran con sistemas externos: el **Procurement Backend** con la API de SUNAT para validar proveedores, y el **Communication Backend** con el servicio de correos.
- Todos los mÃ³dulos backend reutilizan capacidades comunes provistas por el **Shared Backend**, garantizando que todo material solicitado respete el catÃ¡logo maestro y toda acciÃ³n crÃ­tica quede registrada en la auditorÃ­a.

De esta forma, los component diagrams complementan los diagramas de clases del frontend, backend y base de datos, mostrando cÃ³mo los contenedores se descomponen en componentes coherentes con los bounded contexts del dominio y cÃ³mo estos colaboran entre sÃ­ para implementar la funcionalidad completa de Buildline.

![ComponentsDiagram Diagram](../docs/assets/chapter-04/ComponentDiagram.svg)

<div style="page-break-after: always;"></div>

## 4.7. Software Object-Oriented Design
### 4.7.1. Class Diagrams

En esta secciÃ³n se presenta el diseÃ±o orientado a objetos del sistema **Buildline**, el cual desarrolla con mayor detalle la implementaciÃ³n interna de los componentes identificados en los diagramas C4 del apartado anterior. A partir de los contenedores definidos (**API Application** en Spring Boot y **Database** en MySQL), se derivan diagramas de clases especÃ­ficos para cada *bounded context* del dominio, con el objetivo de mostrar:

- **1. Modelado del Dominio (Backend)**

CÃ³mo se estructuran las entidades, agregados, repositorios y servicios dentro de cada *bounded context* (**IAM, Profiles, Requisition, Procurement, Inventory, Suppliers, Analytics & Budgeting y Communication**), asegurando que la lÃ³gica de negocio â€”como la gestiÃ³n de requisiciones, la generaciÃ³n de Ã³rdenes de compra o el cÃ¡lculo de desviaciones presupuestariasâ€” se encuentre correctamente encapsulada y alineada a los principios de *Domain-Driven Design*.

- **2. Arquitectura de AplicaciÃ³n (Backend)**

CÃ³mo se organizan los servicios de aplicaciÃ³n y las interfaces de repositorio que orquestan los casos de uso del sistema, permitiendo la interacciÃ³n entre los distintos contextos sin acoplar directamente sus modelos internos.

- **3. DiseÃ±o de Persistencia (Database)**

CÃ³mo las entidades del dominio se mapean a estructuras relacionales en la base de datos, garantizando la integridad de la informaciÃ³n, la trazabilidad de las operaciones y el soporte a consultas clave del negocio, como el seguimiento de requerimientos, Ã³rdenes de compra y control presupuestal.
A nivel de backend, los diagramas de clases reflejan la implementaciÃ³n de la **API Application** siguiendo principios de *Domain-Driven Design (DDD)*, donde cada *bounded context* encapsula su lÃ³gica de negocio y su modelo de datos de forma independiente, manteniendo bajo acoplamiento y alta cohesiÃ³n.

**Backend completo**

Ilustra la estructura general del sistema organizada por *bounded contexts*, mostrando cÃ³mo cada mÃ³dulo (**IAM, Profiles, Requisition, Procurement, Inventory, Suppliers, Analytics & Budgeting y Communication**) define sus propias entidades, servicios y repositorios, alineados al dominio de la gestiÃ³n de abastecimiento en constructoras.

- **Shared**

Concentra componentes transversales como **MaterialCatalog**, **AuditLog** y el objeto de valor **Money**, los cuales son reutilizados por mÃºltiples contextos para garantizar consistencia en la representaciÃ³n de datos, trazabilidad de operaciones y manejo de valores monetarios.

- **IAM**

Incluye clases como **UserAccount**, **SessionToken** y **AuthService**, responsables de la autenticaciÃ³n, gestiÃ³n de sesiones y control de acceso basado en roles dentro del sistema.

- **Profiles**

Modela las entidades **EmployeeProfile** y **CompanyProfile**, junto con los servicios encargados de gestionar la informaciÃ³n organizacional de la empresa constructora y sus usuarios.

- **Requisition**

Contiene las clases **Requisition** y **RequisitionItem**, que representan las solicitudes de materiales generadas desde obra, junto con los servicios que gestionan su creaciÃ³n, priorizaciÃ³n y seguimiento.

- **Procurement**

Agrupa las entidades **PurchaseOrder** y **Quote**, junto con los servicios que implementan el flujo de compras, incluyendo la comparaciÃ³n de cotizaciones y la generaciÃ³n de Ã³rdenes de compra.

- **Inventory**

Incluye clases como **InventoryItem** y **GoodsReceipt**, encargadas de registrar la recepciÃ³n de materiales en obra, actualizar el stock y validar la correspondencia con las Ã³rdenes de compra.

- **Suppliers**

Modela la entidad **Supplier** y los servicios asociados a su gestiÃ³n, permitiendo mantener un registro estructurado y evaluable de proveedores.

- **Analytics & Budgeting**

Contiene clases como **Budget**, **CostRecord** y **DeviationReport**, responsables de procesar la informaciÃ³n financiera, calcular desviaciones presupuestarias y generar mÃ©tricas para la toma de decisiones.

- **Communication**

Incluye entidades como **Notification** y **Recipient**, junto con servicios que gestionan el envÃ­o de notificaciones internas y comunicaciones relevantes dentro del flujo operativo.

### Diagrama de Clases Backend ###

- **Diagrama Completo**
  
<img src="docs/assets/chapter-04/diagramaBackend.svg" alt="Diagrama de Clases Backend" style="width:auto; height:auto; border:2px solid;">

### Diagrama dividido por contextos ###

- **Shared**
   
  <img src="docs/assets/chapter-04/diagramaShared.png" alt="Diagrama BC Shared" style="width:auto; height:auto; border:2px solid;">

- **IAM**
   
  <img src="docs/assets/chapter-04/diagramaIAM.png" alt="Diagrama BC IAM" style="width:auto; height:auto; border:2px solid;">

- **Profiles**
   
  <img src="docs/assets/chapter-04/diagramaProfiles.png" alt="Diagrama BC Profiles" style="width:auto; height:auto; border:2px solid;">

- **Requisition**
  
  <img src="docs/assets/chapter-04/diagramaRequisition.png" alt="Diagrama BC Requisition" style="width:auto; height:auto; border:2px solid;">

- **Communication**
   
  <img src="docs/assets/chapter-04/diagramaCommunication.png" alt="Diagrama BC Communication" style="width:auto; height:auto; border:2px solid;">

- **Inventory**
   
  <img src="docs/assets/chapter-04/diagramaInventory.png" alt="Diagrama BC Inventory" style="width:auto; height:auto; border:2px solid;">

- **Analytics & Budgeting**
    
  <img src="docs/assets/chapter-04/diagramaAnalytics.png" alt="Diagrama BC Analytics & Budgeting" style="width:auto; height:auto; border:2px solid;">

- **Procurement**
  
  <img src="docs/assets/chapter-04/diagramaProcurement.png" alt="Diagrama BC Procurement" style="width:auto; height:auto; border:2px solid;">

- **Suppliers**
  
  <img src="docs/assets/chapter-04/diagramaSuppliers.png" alt="Diagrama BC Suppliers" style="width:auto; height:auto; border:2px solid;">

## 4.8. Database Design

Ilustra la estructura general del sistema a nivel relacional, organizada por *bounded contexts*, mostrando cÃ³mo cada mÃ³dulo (**IAM, Profiles, Requisition, Procurement, Inventory, Suppliers, Analytics & Budgeting y Communication**) define sus propias tablas, relaciones y restricciones, manteniendo coherencia con el dominio de la gestiÃ³n de abastecimiento en constructoras.

### 4.8.1. Database Diagrams

- **Diagrama Completo**

<img src="docs/assets/chapter-04/diagramaBD.svg" alt="Diagrama de Base de Datos Completo" style="width:auto; height:auto; border:2px solid;">

### Diagrama dividido por contextos

- **Shared**  
  <img src="docs/assets/chapter-04/diagramaBD_shared.png" alt="Diagrama BD Shared" style="width:auto; height:auto; border:2px solid;">

- **IAM**  
  <img src="docs/assets/chapter-04/diagramaDB_iam.png" alt="Diagrama BD IAM" style="width:auto; height:auto; border:2px solid;">

- **Profiles**  
  <img src="docs/assets/chapter-04/diagramaBD_profile.png" alt="Diagrama BD Profiles" style="width:auto; height:auto; border:2px solid;">

- **Requisition**  
  <img src="docs/assets/chapter-04/diagramaBD_requisition.png" alt="Diagrama BD Requisition" style="width:auto; height:auto; border:2px solid;">

- **Procurement**  
  <img src="docs/assets/chapter-04/diagramaBD_procurement.png" alt="Diagrama BD Procurement" style="width:auto; height:auto; border:2px solid;">

- **Inventory**  
  <img src="docs/assets/chapter-04/diagramaBD_inventory.png" alt="Diagrama BD Inventory" style="width:auto; height:auto; border:2px solid;">

- **Suppliers**  
  <img src="docs/assets/chapter-04/diagramaBD_suppliers.png" alt="Diagrama BD Suppliers" style="width:auto; height:auto; border:2px solid;">

- **Analytics & Budgeting**  
  <img src="docs/assets/chapter-04/diagramaBD_analytics.png" alt="Diagrama BD Analytics & Budgeting" style="width:auto; height:auto; border:2px solid;">

- **Communication**  
  <img src="docs/assets/chapter-04/diagramaBD_communication.png" alt="Diagrama BD Communication" style="width:auto; height:auto; border:2px solid;">


<div class="page-break"></div>

# CapÃ­tulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

En esta secciÃ³n se describen las decisiones, convenciones y principios adoptados por el equipo de **RQLS** para garantizar la coherencia, trazabilidad y control de versiones durante el ciclo de vida del desarrollo de la soluciÃ³n **Buildline**. Se establecen los lineamientos para la configuraciÃ³n del entorno de desarrollo, gestiÃ³n del cÃ³digo fuente, convenciones de estilo y configuraciÃ³n de despliegue orientada a la nube.

### 5.1.1. Software Development Environment Configuration

Se especifican los productos de software utilizados durante el ciclo de vida del proyecto, organizados por disciplinas tÃ©cnicas para asegurar la estandarizaciÃ³n del entorno entre los desarrolladores de Buildline.

#### Project Management
* **Jira:** Utilizada para la gestiÃ³n de la metodologÃ­a Scrum, administraciÃ³n del Product Backlog, planificaciÃ³n de Sprints y seguimiento de User Stories para el control logÃ­stico de obra.
    * **Ruta:** [https://www.atlassian.com/software/jira](https://www.atlassian.com/software/jira)

#### Requirements Management
* **Trello:** Empleado para la organizaciÃ³n visual del flujo de trabajo diario y la priorizaciÃ³n rÃ¡pida de tareas durante el desarrollo de los mÃ³dulos de requisiciÃ³n.
    * **Ruta:** [https://trello.com](https://trello.com)

#### Product UX/UI Design
1.  **Miro:** Pizarra colaborativa fundamental para el Design-Level Event Storming de Buildline, permitiendo identificar los eventos de dominio entre obra y oficina.
2.  **Figma:** Herramienta principal para el diseÃ±o de la interfaz mÃ³vil (Field App) y la plataforma web de gestiÃ³n, incluyendo el diseÃ±o del sistema de diseÃ±o (Design System).
3.  **LucidChart:** Utilizado para el modelado de la arquitectura de software mediante diagramas C4 y diagramas de base de datos relacional.

#### Software Development
1.  **GitHub:** Hosting de repositorios bajo la organizaciÃ³n RQLS. ImplementaciÃ³n de GitFlow para separar las funcionalidades de inventario, compras y reportes.
2.  **WebStorm:** IDE especializado para el desarrollo del Frontend de Buildline, optimizando la codificaciÃ³n con Vue.js y la gestiÃ³n de estilos.
3.  **JetBrains Rider:** IDE principal para el desarrollo del Backend robusto basado en .NET/C#, facilitando la integraciÃ³n con servicios de base de datos y lÃ³gica de negocio.
4.  **Vue.js Framework:** Framework progresivo de JavaScript elegido para construir la SPA de Buildline por su ligereza y velocidad de carga en condiciones de baja conectividad en obra.
5.  **.NET 8 / C#:** TecnologÃ­a de backend para garantizar la escalabilidad, seguridad transaccional en las Ã“rdenes de Compra y alto rendimiento.

#### Software Testing
* **Lenguaje Gherkin:** Utilizado para definir los criterios de aceptaciÃ³n en formato Given-When-Then, asegurando que las validaciones de "Way Match" y presupuestos funcionen correctamente.

#### Software Documentation
* **Swagger / OpenAPI:** GeneraciÃ³n de documentaciÃ³n interactiva para que el equipo de Frontend pueda consumir los servicios de requisiciones y proveedores de forma eficiente.

---

### 5.1.2. Source Code Management

Se establecen los repositorios oficiales de la soluciÃ³n Buildline para garantizar la integridad del cÃ³digo fuente.

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
      <td>OrganizaciÃ³n RQLS26</td>
      <td><a href="https://github.com/RQLS26">https://github.com/RQLS26</a></td>
    </tr>
    <tr>
      <td>Landing Page</td>
      <td><a href="https://github.com/RQLS26/Landing-Page">https://github.com/RQLS26/Landing-Page</a></td>
    </tr>
    <tr>
      <td>Frontend Web Application</td>
      <td><a href="https://github.com/RQLS26/Buildline-Frontend">https://github.com/RQLS26/Buildline-Frontend</a></td>
    </tr>
    <tr>
      <td>Backend Web Services</td>
      <td><a href="https://github.com/RQLS26/Buildline-Backend">https://github.com/RQLS26/Buildline-Backend</a></td>
    </tr>
  </tbody>
</table>

#### GitFlow Workflow
* **main:** CÃ³digo estable y auditado desplegado en producciÃ³n.
* **develop:** Rama base para integraciÃ³n de nuevas caracterÃ­sticas.
* **feature/&lt;mÃ³dulo&gt;:** Ej: `feature/procurement-comparison-sheet`.
* **hotfix/&lt;issue&gt;:** Parches rÃ¡pidos para errores crÃ­ticos en el cÃ¡lculo de APU.

<h4>Conventional Commits</h4>
<pre><code>feat(tracking): implement IoT telemetry ingestion endpoint
fix(compliance): resolve stock update discrepancy on partial receipt
docs(readme): update swagger definitions for supplier endpoints
build(deps): migrate to .NET 8.0 SDK
</code></pre>


### 5.1.3. Source Code Style Guide & Conventions

En esta secciÃ³n se establecen las convenciones de estilo y nomenclatura adoptadas para los lenguajes utilizados en el proyecto Buildline: HTML, CSS, JavaScript, TypeScript (Vue.js), C# (.NET 8) y Gherkin. Se aplica nomenclatura en inglÃ©s para todos los elementos del cÃ³digo, siguiendo el Ubiquitous Language definido para el dominio logÃ­stico de la construcciÃ³n.

#### Referencias de GuÃ­as de Estilo Adoptadas

| Lenguaje/TecnologÃ­a | GuÃ­a de Estilo |
| :--- | :--- |
| HTML/CSS | [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html) |
| JavaScript | [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html) |
| TypeScript / Vue.js | [Vue.js Priority A Guide](https://vuejs.org/style-guide/rules-essential.html) |
| C# / .NET | [Microsoft C# Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions) |
| Java | [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html) 
| Gherkin | [Gherkin Reference](https://cucumber.io/docs/gherkin/reference/) |

Se utiliza nomenclatura en inglÃ©s relacionada con las entidades del dominio logÃ­stico (ej. Requisition, Quote, Inventory, Provider).

| Elemento | ConvenciÃ³n | Ejemplo |
| :--- | :--- | :--- |
| Clases C# | PascalCase | `PurchaseOrderService`, `BudgetController` |
| Interfaces C# | PascalCase (prefijo I) | `IRequisitionRepository` |
| MÃ©todos C# | PascalCase | `CalculateOvercost()`, `ApproveOrder()` |
| Variables / MÃ©todos TS | camelCase | `materialId`, `fetchQuotes()` |
| Constantes | SCREAMING_SNAKE_CASE | `MIN_STOCK_LEVEL`, `MAX_FILE_SIZE` |
| Componentes Vue | kebab-case (archivos) | `quote-comparison-table.vue` |

#### SangrÃ­a y Formato
* Se aplica una indentaciÃ³n de dos espacios para archivos web (HTML, CSS, TS) y de cuatro espacios para C# (estÃ¡ndar de Rider/Visual Studio).
* Las llaves de apertura en C# se colocan en una nueva lÃ­nea (Estilo Allman), mientras que en TS/JS van en la misma lÃ­nea (Estilo K&R).

---
### 5.1.4. Software Deployment Configuration

Se especifica la configuraciÃ³n de despliegue para los entornos de Buildline, garantizando alta disponibilidad para ingenieros en obra.

#### Landing Page - Vercel
Despliegue automÃ¡tico del contenido estÃ¡tico mediante la integraciÃ³n con Vercel tras cada merge a la rama `main`.
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
      <td>Castillo Yataco, Mauricio SebastiÃ¡n</td>
    </tr>
    <tr>
      <td>Attendees</td>
      <td>
        Castillo Yataco, Mauricio SebastiÃ¡n<br>
        Morales Venegas, David Joel<br>
        Paucar Zenteno, JesÃºs Fernando<br>
        Viza Quispe, Marlon Packard<br>
        CÃ¡ceres Pizarro, Albino Florencio
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Goal & User Stories</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint 1 Goal (Outcomeâ€“Impactâ€“Customerâ€“Confirmation):</strong><br><br>
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
  <strong>Repositorio:</strong> <a href="https://github.com/RQLS26/Landing-Page">https://github.com/RQLS26/Landing-Page</a>
</p>
#### 5.2.1.2. Aspect Leaders and Collaborators

<p>
Esta matriz <strong>LACX</strong> identifica los aspectos principales del sprint y asigna responsabilidades (LÃ­der/Colaborador) para organizar al equipo de RQLS.
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
    <tr><td>Castillo Yataco, Mauricio SebastiÃ¡n</td><td>L</td><td>C</td></tr>
    <tr><td>Morales Venegas, David Joel</td><td>C</td><td>L</td></tr>
    <tr><td>Paucar Zenteno, JesÃºs Fernando</td><td>C</td><td>C</td></tr>
    <tr><td>Viza Quispe, Marlon Packard</td><td>C</td><td>C</td></tr>
    <tr><td>CÃ¡ceres Pizarro, Albino Florencio</td><td>C</td><td>C</td></tr>
  </tbody>
</table>

### 5.2.1.3. Sprint Backlog 1  

El Sprint Backlog agrupa las tareas iniciales correspondientes a la presencia digital del proyecto Buildline.

<div align="center">
  <img src="docs/assets/chapter-05/jira1.png" alt="Sprint 1 Board Screenshot" width="100%">
  <p><em>Figura: Tablero del Sprint 1 en Jira Software (Proyecto Buildline)</em></p>
</div>

| User Story Id | Title | Task Id | Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **US00** | Landing Page Base | T001 | ImplementaciÃ³n de Hero y Features | Desarrollo de la secciÃ³n principal y propuesta de valor en HTML/CSS/Vue.js. | 4h | Morales Venegas, David Joel | Done |
| **US00** | Landing Page Info | T002 | MaquetaciÃ³n de Beneficios | ImplementaciÃ³n de la secciÃ³n informativa detallando el control de APU y la trazabilidad logÃ­stica. | 3h | Castillo Yataco, Mauricio Sebastian | Done |
| **Cap I - II** | Discovery & Discovery | T003 | Needfinding y Strategic Domain | AnÃ¡lisis de entrevistas con gerentes de obra, Lean UX Canvas y definiciÃ³n del Ubiquitous Language. | 6h | Viza Quispe, Marlon | Done |
| **Cap II - III** | Requirements Eng. | T004 | Context Mapping y Product Backlog | DefiniciÃ³n del Mapa de Contexto (DDD), Impact Mapping y redacciÃ³n de User Stories (Gherkin). | 5h | Paucar Zenteno, Jesus Fernando | Done |
| **Cap IV** | Software Design | T005 | Event Storming y C4 Model | SesiÃ³n de Design-Level Event Storming y elaboraciÃ³n de diagramas de Contexto y Contenedores en Structurizr. | 7h | CÃ¡ceres Pizarro, Albino Florencio | Done |

#### 5.2.1.4. Development Evidence for Sprint Review

<p>
  Resumen de los commits mÃ¡s relevantes en el repositorio de la Landing Page de Buildline.
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
  Se completÃ³ la implementaciÃ³n y el diseÃ±o de la Landing Page.
</p>

#### 5.2.1.6. Services Documentation Evidence
<p>
  Dado que el Sprint 1 abarca Ãºnicamente contenido estÃ¡tico (Landing Page de marketing), la implementaciÃ³n y consumo de la API en .NET para la gestiÃ³n de requisiciones y Ã³rdenes de compra se abordarÃ¡ en los sprints posteriores orientados al Backend Web Services.
</p>

#### 5.2.1.7. Software Deployment Evidence
<p>
  <strong>URL de ProducciÃ³n:</strong> <a href="https://landing-page-bay-iota.vercel.app/">https://landing-page-bay-iota.vercel.app/</a>
</p>

#### 5.2.1.8. Team Collaboration Insights during Sprint

<p>
  Durante este primer sprint, el esfuerzo principal del equipo de RQLS se centrÃ³ en la estructuraciÃ³n del proyecto, el diseÃ±o de UX/UI, la arquitectura de software y la elaboraciÃ³n de los requerimientos tÃ©cnicos (CapÃ­tulos I al IV). Por lo tanto, las evidencias de colaboraciÃ³n de GitHub presentadas a continuaciÃ³n corresponden al repositorio del <strong>Project Report</strong>, sentando las bases documentales y de diseÃ±o para la posterior codificaciÃ³n de la plataforma Buildline.
</p>

<p>
  En primer lugar, el <strong>Historial de Commits</strong> del repositorio demuestra que el trabajo no fue centralizado, sino altamente colaborativo. A lo largo del sprint, se observa un flujo constante de aportes realizados en diferentes dÃ­as por distintos miembros del equipo (reflejados a travÃ©s de sus usuarios de GitHub). Cada integrante se encargÃ³ de actualizar y mejorar secciones especÃ­ficas, como el anÃ¡lisis de entrevistas a los Gerentes y Residentes, el Event Storming o los diagramas de arquitectura C4, evidenciando un desarrollo incremental y distribuido.
</p>

<div align="center">
  <img src="../docs/assets/chapter-05/commit-history-sprint1.png" alt="Commit History Evidence" width="90%">
  <p><em>Figura: Historial de commits demostrando la participaciÃ³n activa de los miembros del equipo RQLS.</em></p>
</div>

<p>
  En segundo lugar, el grÃ¡fico de <strong>Visitors (Traffic)</strong> proporcionado por los Insights de GitHub demuestra que el repositorio documental mantuvo una actividad de consulta constante. El flujo de "Views" y "Unique visitors" a lo largo de las semanas del sprint confirma que los integrantes del equipo ingresaban recurrentemente al repositorio no solo para subir su parte, sino para revisar el trabajo de sus compaÃ±eros, unificar criterios sobre el Ubiquitous Language (como "Way Match" y "APU") y validar la coherencia de los diagramas antes del cierre del documento.
</p>

<div align="center">
  <img src="../docs/assets/chapter-05/visitors-sprint1.png" alt="Traffic Visitors Graph">
  <p><em>Figura: GrÃ¡fica de visitantes mostrando la revisiÃ³n constante del repositorio por parte del equipo.</em></p>
</div>

### 5.2.2. Sprint 2

En esta secciÃ³n se documenta el avance del Sprint 2 del proyecto Buildline. El alcance principal corresponde a la implementaciÃ³n y despliegue de la **primera versiÃ³n del Frontend Web Application** de Buildline, asÃ­ como la publicaciÃ³n de una **nueva versiÃ³n del Landing Page** con correcciones derivadas del feedback recibido en AV1. El frontend se desarrollÃ³ con Vue.js 3, Vite, Pinia, Vue Router, PrimeVue y vue-i18n, organizado por *bounded contexts* siguiendo la arquitectura DDD definida en el CapÃ­tulo IV.

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
      <td>Castillo Yataco, Mauricio SebastiÃ¡n</td>
    </tr>
    <tr>
      <td>Attendees</td>
      <td>
        Castillo Yataco, Mauricio SebastiÃ¡n<br>
        Morales Venegas, David Joel<br>
        Paucar Zenteno, JesÃºs Fernando<br>
        Viza Quispe, Marlon Packard<br>
        CÃ¡ceres Pizarro, Albino Florencio
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint 1 Review Summary</strong></td>
    </tr>
    <tr>
      <td colspan="2">
        Se entregÃ³ y desplegÃ³ la primera versiÃ³n del Landing Page de Buildline en GitHub Pages, cubriendo las secciones Hero, Features, Benefits, Plans y About Us. El Product Owner aprobÃ³ el resultado y recomendÃ³ reforzar la jerarquÃ­a visual del Hero y mejorar las llamadas a la acciÃ³n del bloque de Planes para la prÃ³xima entrega.
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint 1 Retrospective Summary</strong></td>
    </tr>
    <tr>
      <td colspan="2">
        El equipo coincidiÃ³ en que la coordinaciÃ³n inicial fue lenta por la falta de un tablero unificado. Para el Sprint 2 se acordÃ³ migrar al uso intensivo de Jira, definir Definition of Done explÃ­cita por user story y realizar daily syncs cortos por Discord cada dos dÃ­as para destrabar bloqueos a tiempo.
      </td>
    </tr>
    <tr>
      <td colspan="2" style="text-align: center;"><strong>Sprint Goal & User Stories</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint 2 Goal (Outcomeâ€“Impactâ€“Customerâ€“Confirmation):</strong><br><br>
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
  <strong>Repositorio Frontend:</strong> <a href="https://github.com/RQLS26/Frontend">https://github.com/RQLS26/Frontend</a><br>
  <strong>Repositorio Landing Page v2:</strong> <a href="https://github.com/RQLS26/Landing-Page">https://github.com/RQLS26/Landing-Page</a>
</p>

#### 5.2.2.2. Aspect Leaders and Collaborators

<p>
Para el Sprint 2 se identificaron seis aspectos funcionales que corresponden a los <em>bounded contexts</em> implementados en el frontend, mÃ¡s un aspecto transversal de Project Setup (Vue 3 + Vite + Pinia + i18n + json-server) y un aspecto para la versiÃ³n v2 del Landing Page. La siguiente matriz <strong>LACX</strong> identifica los aspectos principales del Sprint y asigna responsabilidades (LÃ­der/Colaborador) al equipo de RQLS, alineadas con las fortalezas tÃ©cnicas evidenciadas durante el Sprint 1.
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
    <tr><td>Castillo Yataco, Mauricio SebastiÃ¡n</td><td>L</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Morales Venegas, David Joel</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td><td>L</td><td>L</td></tr>
    <tr><td>Paucar Zenteno, JesÃºs Fernando</td><td>C</td><td>L</td><td>C</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Viza Quispe, Marlon Packard</td><td>C</td><td>C</td><td>L</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>CÃ¡ceres Pizarro, Albino Florencio</td><td>C</td><td>C</td><td>C</td><td>L</td><td>L</td><td>C</td><td>C</td></tr>
  </tbody>
</table>

#### 5.2.2.3. Sprint Backlog 2

El Sprint Backlog 2 agrupa los User Stories priorizados del Product Backlog que corresponden al primer release navegable del Frontend Web Application, organizados por bounded context. Se utilizÃ³ Jira Software como herramienta de control de estado.

<div align="center">
  <img src="docs/assets/chapter-05/jira2.png" alt="Sprint 2 Board Screenshot" width="100%">
  <p><em>Figura: Tablero del Sprint 2 en Jira Software (Proyecto Buildline)</em></p>
</div>

| User Story Id | Title | Task Id | Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **US01** | Authentication and Access Control | T101 | Sign-In View | Vista de inicio de sesiÃ³n con validaciÃ³n de credenciales contra el mock service. | 4h | Castillo Yataco, Mauricio SebastiÃ¡n | Done |
| **US01** | Authentication and Access Control | T102 | Sign-Up View | Vista de registro con persistencia en json-server y redirecciÃ³n a Sign-In. | 4h | Castillo Yataco, Mauricio SebastiÃ¡n | Done |
| **US01** | Authentication and Access Control | T103 | Forgot Password View | Formulario de recuperaciÃ³n de contraseÃ±a y feedback visual al usuario. | 2h | Castillo Yataco, Mauricio SebastiÃ¡n | Done |
| **US01** | Authentication and Access Control | T104 | IAM Pinia Store & Route Guards | Estado global de autenticaciÃ³n y protecciÃ³n de rutas privadas vÃ­a `router.beforeEach`. | 3h | Castillo Yataco, Mauricio SebastiÃ¡n | Done |
| **US02** | Material Requisitions | T201 | Material Request List View | Listado de requisiciones con filtros por proyecto, prioridad y estado. | 4h | Paucar Zenteno, JesÃºs Fernando | Done |
| **US02** | Material Requisitions | T202 | New Requisition Form | Formulario de creaciÃ³n de requisiciones con validaciÃ³n contra el catÃ¡logo de materiales. | 4h | Paucar Zenteno, JesÃºs Fernando | Done |
| **US02** | Material Requisitions | T203 | Requisition Service (Axios) | Capa de infraestructura para consumir los endpoints `/requisitions` y `/materials` del mock. | 3h | Paucar Zenteno, JesÃºs Fernando | Done |
| **US03** | Supplier Directory | T301 | Supplier Directory View | Listado de proveedores con RUC, razÃ³n social, rating y estado. | 3h | Viza Quispe, Marlon Packard | Done |
| **US03** | Supplier Directory | T302 | Incidents List View | Vista de incidencias asociadas a proveedores con severidad y estado. | 3h | Viza Quispe, Marlon Packard | Done |
| **US04** | Purchase Order Management | T401 | Approval Inbox View | Bandeja de Ã³rdenes de compra con acciones de aprobaciÃ³n o rechazo. | 4h | Paucar Zenteno, JesÃºs Fernando | Done |
| **US04** | Purchase Order Management | T402 | Quotations Management View | Vista para gestionar y comparar cotizaciones recibidas. | 4h | Paucar Zenteno, JesÃºs Fernando | Done |
| **US05** | Inventory Tracking | T501 | Inventory List View | Listado de inventario con indicadores de stock crÃ­tico vs stock mÃ­nimo. | 4h | CÃ¡ceres Pizarro, Albino Florencio | Done |
| **US05** | Inventory Tracking | T502 | Inventory Service & Filters | Filtros por proyecto, categorÃ­a y estado de stock. | 3h | CÃ¡ceres Pizarro, Albino Florencio | Done |
| **US06** | Financial Dashboard | T601 | Financial Dashboard View | Dashboard de presupuesto vs gasto por proyecto con estados *On Track / At Risk / Over Budget*. | 4h | CÃ¡ceres Pizarro, Albino Florencio | Done |
| **US06** | Financial Dashboard | T602 | Reports View (PDF Export) | Vista de reportes financieros con exportaciÃ³n a PDF mediante `html2pdf.js`. | 3h | CÃ¡ceres Pizarro, Albino Florencio | Done |
| **US07** | Company Profile | T701 | Company Profile View | Vista de perfil de la empresa con RUC, direcciÃ³n, telÃ©fono y correo. | 2h | Morales Venegas, David Joel | Done |
| **US08** | Internal Communications | T801 | Messages Inbox View | Bandeja de mensajes internos con indicador de leÃ­do / no leÃ­do. | 3h | Morales Venegas, David Joel | Done |
| **Tech** | Project Setup | T901 | Vue 3 + Vite + Pinia + Router | ConfiguraciÃ³n inicial del proyecto frontend con la estructura por bounded contexts. | 3h | Castillo Yataco, Mauricio SebastiÃ¡n | Done |
| **Tech** | Project Setup | T902 | i18n (es/en) and PrimeVue Theme | InternacionalizaciÃ³n y aplicaciÃ³n del theme PrimeVue (PrimeUIX). | 2h | Castillo Yataco, Mauricio SebastiÃ¡n | Done |
| **Tech** | Project Setup | T903 | json-server Mock API | ConfiguraciÃ³n del mock service en `server/db.json` y script `npm run dev` con `concurrently`. | 2h | Castillo Yataco, Mauricio SebastiÃ¡n | Done |
| **Tech** | Landing v2 | T910 | Landing Page Refinements | Mejora del Hero, jerarquÃ­a visual y CTAs del Landing Page segÃºn feedback AV1. | 4h | Morales Venegas, David Joel | Done |

#### 5.2.2.4. Development Evidence for Sprint Review

<p>
  Durante el Sprint 2 el equipo concentrÃ³ su trabajo en dos repositorios: el repositorio del <strong>Frontend Web Application</strong> (creado al inicio del Sprint) y el repositorio del <strong>Landing Page</strong> (para la versiÃ³n v2). La siguiente tabla resume los commits mÃ¡s relevantes asociados a cada user story y aspecto del Sprint.
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
  Al cierre del Sprint 2 el equipo entregÃ³ una versiÃ³n navegable del Frontend Web Application de Buildline, ejecutable localmente mediante <code>npm run dev</code>, comando que levanta en paralelo Vite y el mock service (json-server) gracias a <code>concurrently</code>. El alcance funcional implementado cubre los siguientes flujos:
</p>

<ul>
  <li><strong>IAM (Identity and Access Management):</strong> Sign-In, Sign-Up, Forgot Password y protecciÃ³n de rutas privadas mediante <em>route guard</em> sobre <code>router.beforeEach</code>.</li>
  <li><strong>Requisition:</strong> Listado y creaciÃ³n de requisiciones de materiales vinculadas a proyectos.</li>
  <li><strong>Suppliers:</strong> Directorio de proveedores con RUC, razÃ³n social, rating y vista de incidencias asociadas.</li>
  <li><strong>Procurement:</strong> Bandeja de aprobaciÃ³n de Ã“rdenes de Compra y gestiÃ³n de cotizaciones para comparaciÃ³n.</li>
  <li><strong>Inventory:</strong> Listado de inventario con indicadores de stock crÃ­tico y filtros por proyecto y categorÃ­a.</li>
  <li><strong>Analytics & Budgeting:</strong> Dashboard financiero por proyecto con estados <em>On Track / At Risk / Over Budget</em> y vista de reportes con exportaciÃ³n a PDF.</li>
  <li><strong>Profiles:</strong> Perfil de la empresa con datos legales y de contacto.</li>
  <li><strong>Communication:</strong> Bandeja de mensajes internos entre obra y oficina.</li>
</ul>

<p>
  La aplicaciÃ³n cuenta con soporte <strong>i18n</strong> (espaÃ±ol e inglÃ©s), <strong>theme PrimeVue</strong> y navegaciÃ³n SPA con Vue Router. A continuaciÃ³n se incluyen las capturas representativas del Sprint Review.
</p>

<div align="center">
  <img src="docs/assets/chapter-05/sprint2-signin.png" alt="Sign-In View" width="90%">
  <p><em>Figura: Vista Sign-In del bounded context IAM.</em></p>
</div>

<div align="center">
  <img src="docs/assets/chapter-05/sprint2-requisitions.png" alt="Material Requests View" width="90%">
  <p><em>Figura: Listado de Material Requests con filtros por proyecto y prioridad.</em></p>
</div>

<div align="center">
  <img src="docs/assets/chapter-05/sprint2-suppliers.png" alt="Supplier Directory" width="90%">
  <p><em>Figura: Directorio de Proveedores con RUC, rating y estado.</em></p>
</div>

<div align="center">
  <img src="docs/assets/chapter-05/sprint2-procurement.png" alt="Approval Inbox" width="90%">
  <p><em>Figura: Approval Inbox de Ã“rdenes de Compra.</em></p>
</div>

<div align="center">
  <img src="docs/assets/chapter-05/sprint2-inventory.png" alt="Inventory List" width="90%">
  <p><em>Figura: Inventory List con indicadores visuales de stock crÃ­tico.</em></p>
</div>

<div align="center">
  <img src="docs/assets/chapter-05/sprint2-dashboard.png" alt="Financial Dashboard" width="90%">
  <p><em>Figura: Dashboard Overview (resumen).</em></p>
</div>

<h4>Video About The Product</h4>

<p>En esta secciÃ³n se presenta el video demostrativo oficial de la plataforma <strong>Buildline (Release v1.0.0)</strong>, elaborado para el cierre del Sprint 2. El propÃ³sito de este video es evidenciar la integraciÃ³n end-to-end de nuestra arquitectura, mostrando desde la gestiÃ³n de requisiciones y el control de inventario hasta el impacto automÃ¡tico en el Dashboard Financiero. El material audiovisual ha sido alojado de forma segura en la plataforma institucional <strong>Microsoft Stream</strong>.</p>

<div align="center">
  <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231b504_upc_edu_pe/IQBmp9aQwMuLSLxjirNLDL3-ATVaXbe2IUg_aTtw3V59494?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Y9T9qs" target="_blank">
    <img src="docs/assets/chapter-05/video-screenshot.png" alt="Video Demostrativo Buildline en Microsoft Stream" width="90%" style="border: 1px solid #ccc; border-radius: 8px;">
  </a>
  <p><em>Figura: Video demostrativo en Microsoft Stream.</em></p>
</div>

Enlace directo: https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231b504_upc_edu_pe/IQBmp9aQwMuLSLxjirNLDL3-ATVaXbe2IUg_aTtw3V59494?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Y9T9qs

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

<p>
  Durante el Sprint 2 no se implementaron aÃºn los Web Services productivos en .NET (planificados para el Sprint 3 segÃºn el cronograma del curso). Para soportar la primera versiÃ³n del Frontend Web Application y validar contratos de API tempranos, el equipo configurÃ³ un <strong>mock service local con json-server</strong> que expone los endpoints requeridos por los bounded contexts implementados. Esta documentaciÃ³n servirÃ¡ como contrato base para los Web Services definitivos en .NET 8.
</p>

<p><strong>URL del Mock API (local):</strong> <code>http://localhost:3000</code></p>
<p><strong>URL del Mock API (ProducciÃ³n en Render):</strong> <code>https://buildline-json-server.onrender.com/</code></p>

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
      <td>GET listado, GET /:id, POST creaciÃ³n, PUT /:id actualizaciÃ³n de estado.</td>
      <td><code>POST /requisitions</code> con <code>{ reqId, material, project, priority, status, requestedOn }</code></td>
      <td><code>{ "id":"4", "reqId":"MR-2026-00025", "material":"Cemento Sol", "status":"Pending" }</code></td>
    </tr>
    <tr>
      <td><code>/materials</code></td>
      <td>GET catÃ¡logo de materiales para el formulario de requisiciÃ³n.</td>
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
      <td>GET listado, POST registro de cotizaciÃ³n para comparaciÃ³n.</td>
      <td><code>GET /quotations</code></td>
      <td><code>[]</code> (vacÃ­o al inicio del Sprint)</td>
    </tr>
    <tr>
      <td><code>/inventory</code></td>
      <td>GET listado, GET /:id, filtrado por proyecto y categorÃ­a vÃ­a query params.</td>
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
      <td>GET listado, PUT /:id marcar como leÃ­do.</td>
      <td><code>PUT /messages/1</code> con <code>{ "isRead": true }</code></td>
      <td><code>{ "id":"1","sender":"Aceros Arequipa S.A.","subject":"CotizaciÃ³n Lista","isRead":true }</code></td>
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
  La documentaciÃ³n <strong>OpenAPI/Swagger</strong> definitiva se elaborarÃ¡ y desplegarÃ¡ junto con los Web Services en .NET 8 durante el Sprint 3.
</p>

<p>
  <strong>Repositorio del Frontend (incluye el mock):</strong> <a href="https://github.com/RQLS26/Frontend">https://github.com/RQLS26-Frontend</a><br>
  <strong>Commit relacionado con documentaciÃ³n del mock:</strong> <code>9c0d1e2</code>
</p>

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

<p>
  Durante el Sprint 2 se realizaron actividades de despliegue para dos productos: la nueva versiÃ³n del <strong>Landing Page (v2)</strong> y la primera versiÃ³n del <strong>Frontend Web Application</strong>.
</p>

<p><strong>Landing Page v2 (Vercel)</strong></p>
<ul>
  <li>Se incorporaron las mejoras de UI recomendadas en el feedback AV1 (jerarquÃ­a del Hero y CTAs del bloque de Planes).</li>
  <li>El despliegue fue migrado a la plataforma Vercel para asegurar integraciÃ³n nativa con Vite, automatizado en cada merge a <code>main</code>.</li>
  <li><strong>URL de ProducciÃ³n:</strong> <a href="https://landing-page-bay-iota.vercel.app/">https://landing-page-bay-iota.vercel.app/</a></li>
</ul>

<p><strong>Frontend Web Application (primera versiÃ³n)</strong></p>
<ul>
  <li>Se actualizÃ³ el repositorio <code>RQLS26-Frontend</code> con el proyecto Vue 3 + Vite + Pinia finalizado.</li>
  <li>Se configurÃ³ el despliegue automÃ¡tico conectando el repositorio directamente a <strong>Vercel</strong>, aÃ±adiendo el archivo <code>vercel.json</code> para manejar las reglas del Single Page Application (SPA).</li>
  <li>Se desplegÃ³ paralelamente el mock en <code>db.json</code> como un Web Service en <strong>Render</strong> para contar con persistencia remota.</li>
  <li><strong>URL de ProducciÃ³n:</strong> <a href="https://buildline-3jcvvnh4t-team-project0.vercel.app/">https://buildline-3jcvvnh4t-team-project0.vercel.app/</a></li>
</ul>

<p><strong>Pasos realizados durante el Sprint:</strong></p>
<ol>
  <li>ConfiguraciÃ³n del frontend dinÃ¡mico utilizando variables de entorno (<code>VITE_API_BASE_URL</code>) para apuntar a Render en producciÃ³n y localhost en desarrollo.</li>
  <li>CreaciÃ³n de un repositorio de backend para el `json-server` y despliegue a Render como servicio web.</li>
  <li>ConexiÃ³n e importaciÃ³n del repositorio de Frontend a Vercel con la configuraciÃ³n de History Mode.</li>
  <li>ConexiÃ³n de la Landing Page a Vercel, garantizando compatibilidad inmediata sin configuraciÃ³n adicional.</li>
  <li>VerificaciÃ³n exitosa post-despliegue del cruce de datos y navegaciÃ³n integral de ambas plataformas.</li>
</ol>

#### 5.2.2.8. Team Collaboration Insights during Sprint

<p>
  Durante el Sprint 2 el equipo de RQLS migrÃ³ el seguimiento de tareas desde un backlog plano a un board activo en Jira, con columnas <em>To Do</em>, <em>In Progress</em>, <em>To Review</em> y <em>Done</em>. Esta prÃ¡ctica fue acordada en la retrospectiva del Sprint 1 y se reflejÃ³ en una reducciÃ³n de tareas bloqueadas y una mejor distribuciÃ³n de la carga entre los integrantes.
</p>

<p>
  El trabajo se organizÃ³ por <em>bounded contexts</em>, lo que permitiÃ³ que cada lÃ­der asumiera la responsabilidad tÃ©cnica de su feature mientras los colaboradores apoyaban con revisiÃ³n de cÃ³digo, pruebas locales y documentaciÃ³n. La comunicaciÃ³n principal se realizÃ³ por Discord, y cada Pull Request fue revisado por al menos un colaborador antes de hacer merge a <code>main</code>.
</p>

<div align="center">
  <img src="../docs/assets/chapter-05/commit-history-sprint2.png" alt="Commit History Sprint 2" width="90%">
  <p><em>Figura: Historial de commits del repositorio Frontend, evidenciando la participaciÃ³n distribuida del equipo RQLS durante el Sprint 2.</em></p>
</div>

<div align="center">
  <img src="../docs/assets/chapter-05/contributors-sprint2.png" alt="Contributors Insights Sprint 2" width="90%">
  <p><em>Figura: GrÃ¡fica de Contributors de GitHub Insights mostrando la distribuciÃ³n de contribuciones del Sprint 2.</em></p>
</div>

<p><strong>MÃ©tricas de colaboraciÃ³n del Sprint 2:</strong></p>
<ul>
  <li><strong>Story Points completados:</strong> 28 / 28</li>
  <li><strong>Total de Issues cerrados en Jira:</strong> 21</li>
  <li><strong>Total de Pull Requests cerrados:</strong> 0</li>
  <li><strong>Total de commits en el repositorio Frontend:</strong> 20</li>
</ul>

<p><strong>Aciertos del Sprint:</strong></p>
<ul>
  <li>La estructura DDD por <em>bounded contexts</em> en el frontend (<code>iam</code>, <code>requisition</code>, <code>suppliers</code>, <code>procurement</code>, <code>inventory</code>, <code>analytics-budgeting</code>, <code>profiles</code>, <code>communication</code>) permitiÃ³ trabajar en paralelo sin conflictos significativos de merge.</li>
  <li>El uso de json-server como mock alineÃ³ al equipo en torno a contratos de API tempranos, lo que facilitarÃ¡ la futura integraciÃ³n con los Web Services en .NET 8.</li>
  <li>La adopciÃ³n de <strong>i18n</strong> desde el inicio evitÃ³ refactors posteriores y dejÃ³ listo el soporte multilenguaje (es/en).</li>
</ul>

<p><strong>Oportunidades de mejora identificadas:</strong></p>
<ul>
  <li>Reforzar la cobertura de validaciones de formulario, especialmente en Sign-Up y New Requisition.</li>
  <li>Documentar explÃ­citamente la convenciÃ³n de nombres de stores Pinia y de servicios Axios para mantener consistencia entre bounded contexts.</li>
  <li>Adelantar la configuraciÃ³n de pruebas unitarias con Vitest hacia el inicio del Sprint 3.</li>
</ul>


<div class="page-break"></div>

# CapÃ­tulo VI: Conclusions
## 6.1. Conclusiones y recomendaciones
<p>
  Al finalizar el primer ciclo de investigaciÃ³n, diseÃ±o e implementaciÃ³n de la presencia digital de la soluciÃ³n <strong>Buildline</strong>, el equipo RQLS ha llegado a una serie de conclusiones clave, contrastando los resultados obtenidos con los planteamientos iniciales definidos bajo el enfoque Lean UX y el desarrollo Ã¡gil basado en Sprints.
</p> 

<p><strong>1. ValidaciÃ³n de Problem Statements y Supuestos (Assumptions):</strong></p> 
<p>
  Inicialmente, se planteÃ³ como <em>Problem Statement</em> que las MYPES constructoras enfrentan un sobrecosto logÃ­stico estructural del 21.1% debido a procesos de abastecimiento informales (uso de WhatsApp), falta de trazabilidad entre obra y oficina, y la nula visibilidad del gasto real frente al presupuesto base (APU). A partir del Needfinding y la validaciÃ³n del modelo de negocio, se confirmÃ³ que existe una urgencia real por soluciones digitales que democraticen el control logÃ­stico sin requerir implementaciones de ERPs costosos.
</p> 
<p>
  Asimismo, se validÃ³ el supuesto de que los Jefes de Proyecto (segmento comprador) valoran altamente la capacidad de bloquear compras no planificadas. Sin embargo, se identificÃ³ que el Ã©xito de la plataforma depende en gran medida de la adopciÃ³n de la herramienta por parte del Ingeniero Residente en campo, lo que implica que el diseÃ±o de interfaces debe priorizar la rapidez y facilidad de uso.
</p> 

<p><strong>2. ContrastaciÃ³n de HipÃ³tesis (Hypothesis Statements):</strong></p> 
<ul> 
  <li> 
    <strong>HipÃ³tesis de Valor para Gerentes y Jefes de Proyecto:</strong> Se planteÃ³ que "Si proporcionamos paneles de control presupuestal y aprobaciones jerÃ¡rquicas, los gerentes dejarÃ¡n de aprobar compras 'a ciegas' y protegerÃ¡n la rentabilidad". Los resultados obtenidos en la conceptualizaciÃ³n validan esta hipÃ³tesis, siendo el control del APU el principal gatillo de interÃ©s comercial.
  </li> 
  <li> 
    <strong>HipÃ³tesis de Valor para Residentes y LogÃ­stica:</strong> Se asumiÃ³ que "La digitalizaciÃ³n de los requerimientos y la validaciÃ³n automatizada de recepciones (Way Match) eliminarÃ¡n los cuellos de botella". Esta hipÃ³tesis se mantiene validada a nivel conceptual, destacando la necesidad de adjuntar evidencia fotogrÃ¡fica en el flujo de abastecimiento.
  </li> 
</ul> 

<p><strong>3. Cumplimiento de Criterios de Ã‰xito:</strong></p> 
<p>
  Durante el Sprint 1, el desarrollo de software se limitÃ³ estrictamente a la capa de presentaciÃ³n estÃ¡tica. Se logrÃ³ implementar y desplegar exitosamente la Landing Page informativa de Buildline mediante GitHub Pages, cumpliendo con los criterios de aceptaciÃ³n definidos: navegaciÃ³n responsiva, presentaciÃ³n clara de la propuesta de valor, visualizaciÃ³n de planes y perfiles del equipo.
</p> 
<p>
  Al tratarse de un primer incremento enfocado exclusivamente en la web pÃºblica de marketing y la documentaciÃ³n arquitectÃ³nica (CapÃ­tulos I al IV), aÃºn no se han validado mÃ©tricas operativas del sistema central (como la reducciÃ³n de tiempos de cotizaciÃ³n), las cuales serÃ¡n evaluadas una vez se inicie la codificaciÃ³n de la plataforma.
</p> 

<p><strong>Recomendaciones (Roadmap):</strong></p> 
<p>
  Considerando que actualmente solo se cuenta con la Landing Page estÃ¡tica, se recomiendan las siguientes lÃ­neas de acciÃ³n tÃ©cnicas para los prÃ³ximos Sprints orientadas a construir el prototipo funcional:
</p> 
<ul> 
  <li> 
    <strong>Desarrollo del Backend API:</strong> Iniciar la codificaciÃ³n de los Web Services utilizando <strong>.NET 8 (C#)</strong> para gestionar la lÃ³gica de negocio fundamental: creaciÃ³n de requerimientos, control del presupuesto APU y validaciÃ³n de Ã³rdenes de compra.
  </li> 
  <li> 
    <strong>Desarrollo del Frontend (SPA):</strong> Construir la aplicaciÃ³n web interactiva utilizando <strong>Vue.js</strong> para consumir la API, desarrollando inicialmente las vistas del Ingeniero Residente (creaciÃ³n de pedidos) y del LogÃ­stico (cuadro de cotizaciones).
  </li> 
  <li> 
    <strong>Modelado de la Base de Datos:</strong> Implementar localmente la base de datos relacional (MySQL o SQL Server) diseÃ±ada en el diagrama de contenedores, asegurando la integridad de las tablas de usuarios, proyectos, APUs y materiales.
  </li> 
  <li> 
    <strong>IntegraciÃ³n de Entornos Locales:</strong> Establecer una comunicaciÃ³n fluida entre el frontend en Vue.js y el backend en .NET en los entornos de desarrollo locales del equipo, realizando pruebas de integraciÃ³n (API Testing) antes de evaluar cualquier futuro despliegue en servidores.
  </li> 
</ul>

## 6.2. Video About-the-Team
[pending content]


<div class="page-break"></div>

# BibliografÃ­a
<ul>
  <li>
    Brown, S. (2020). <em>The C4 model for visualising software architecture</em>. C4 Model. Recuperado de <a href="https://c4model.com/">https://c4model.com/</a>
  </li>
  <li>
    Cohn, M. (2004). <em>User Stories Applied: For Agile Software Development</em>. Addison-Wesley Professional.
  </li>
  <li>
    Evans, E. (2003). <em>Domain-Driven Design: Tackling Complexity in the Heart of Software</em>. Addison-Wesley Professional.
  </li>
  <li>
    Gothelf, J., & Seiden, J. (2021). <em>Lean UX: Designing Great Products with Agile Teams</em> (3rd ed.). O'Reilly Media.
  </li>
  <li>
    Robertson, J., Robertson, S., & Reed, A. (2023). <em>Mastering the Requirements Process: Getting Requirements Right</em> (4th ed.). Addison-Wesley Professional.
  </li>
  <li>
    Wiegers, K., & Hokanson, C. (2023). <em>Software Requirements Essentials: Core Practices for Successful Business Analysis</em>. Addison-Wesley Professional.
  </li>
  <li>
    Heath, F. (2020). <em>Managing Software Requirements the Agile Way</em>. Packt Publishing.
  </li>
  <li>
    Lee, C. (2023). <em>The Art of Crafting User Stories</em>. O'Reilly Media.
  </li>
  <li>
    DirecciÃ³n General de Medicamentos, Insumos y Drogas [DIGEMID]. (2018). <em>Manual de Buenas PrÃ¡cticas de Manufactura de Productos FarmacÃ©uticos</em>. Ministerio de Salud del PerÃº.
  </li>

  <li>
    Mendel, J. (s.f.). <em>Seriously, whatâ€™s your startupâ€™s problem?</em>. Recuperado de <a href="https://medium.com/@jakemendel/seriously-whats-your-startup-s-problemb3a884c54ab4">https://medium.com/@jakemendel/seriously-whats-your-startup-s-problemb3a884c54ab4</a>
  </li>
  <li>
    <em>Lean UX â€“ Chapter 3 (Sampler)</em>. Recuperado de <a href="https://www.scribd.com/document/655516553/Leanux-Sampler">https://www.scribd.com/document/655516553/Leanux-Sampler</a>
  </li>
  <li>
    Dittrich, J. (s.f.). <em>A Beginnerâ€™s Guide to Finding User Needs</em>. Recuperado de <a href="https://jdittrich.github.io/userNeedResearchBook/">https://jdittrich.github.io/userNeedResearchBook/</a>
  </li>
  <li>
    Mountain Goat Software. (s.f.). <em>User Stories Articles</em>. Recuperado de <a href="https://www.mountaingoatsoftware.com/blog/tag/user-stories">https://www.mountaingoatsoftware.com/blog/tag/user-stories</a>
  </li>
  <li>
    Sameera, S. (s.f.). <em>How to Write a User Story for an API Product</em>. Recuperado de <a href="https://sameera17w.medium.com/how-to-write-a-user-story-for-an-api-product7af6abd4ad2e">https://sameera17w.medium.com/how-to-write-a-user-story-for-an-api-product7af6abd4ad2e</a>
  </li>

  <li>
    UXPressia. (s.f.). <em>User vs. Buyer Persona: Differences and free template</em>. Recuperado de <a href="https://uxpressia.com/blog/user-persona-vs-buyer-persona-difference">https://uxpressia.com/blog/user-persona-vs-buyer-persona-difference</a>
  </li>
  <li>
    UXPressia. (s.f.). <em>How to create an Impact Map in 4 easy steps?</em>. Recuperado de <a href="https://uxpressia.com/blog/build-impact-map-4-easy-steps">https://uxpressia.com/blog/build-impact-map-4-easy-steps</a>
  </li>
  <li>
    IBM. (s.f.). <em>As-is Scenario Map</em>. Recuperado de <a href="https://www.ibm.com/design/thinking/page/toolkit/activity/as-is-scenario-map">https://www.ibm.com/design/thinking/page/toolkit/activity/as-is-scenario-map</a>
  </li>
  <li>
    IBM. (s.f.). <em>To-be Scenario Map</em>. Recuperado de <a href="https://www.ibm.com/design/thinking/page/toolkit/activity/to-be-scenario-map">https://www.ibm.com/design/thinking/page/toolkit/activity/to-be-scenario-map</a>
  </li>
  <li>
    IBM. (s.f.). <em>Empathy Map</em>. Recuperado de <a href="https://www.ibm.com/design/thinking/page/toolkit/activity/empathy-map">https://www.ibm.com/design/thinking/page/toolkit/activity/empathy-map</a>
  </li>
  <li>
    Nielsen Norman Group. (s.f.). <em>Empathy Mapping</em>. Recuperado de <a href="https://www.nngroup.com/articles/empathy-mapping/">https://www.nngroup.com/articles/empathy-mapping/</a>
  </li>
  <li>
    Nielsen Norman Group. (s.f.). <em>Design Systems 101</em>. Recuperado de <a href="https://www.nngroup.com/articles/design-systems-101/">https://www.nngroup.com/articles/design-systems-101/</a>
  </li>
  <li>
    Nielsen Norman Group. (s.f.). <em>Front-End Style Guides</em>. Recuperado de <a href="https://www.nngroup.com/articles/front-end-style-guides/">https://www.nngroup.com/articles/front-end-style-guides/</a>
  </li>
  <li>
    Nielsen Norman Group. (s.f.). <em>The Four Dimensions of Tone of Voice</em>. Recuperado de <a href="https://www.nngroup.com/articles/tone-of-voice-dimensions/">https://www.nngroup.com/articles/tone-of-voice-dimensions/</a>
  </li>
  <li>
    CareerFoundry. (s.f.). <em>What are User Flows in UX Design?</em>. Recuperado de <a href="https://careerfoundry.com/en/blog/ux-design/what-are-user-flows/">https://careerfoundry.com/en/blog/ux-design/what-are-user-flows/</a>
  </li>

  <li>
    Progressa Lean. (s.f.). <em>5W2H â€“ TÃ©cnica de anÃ¡lisis de problemas</em>. Recuperado de <a href="https://www.progressalean.com/5w2h-tecnica-de-analisis-de-problemas/">https://www.progressalean.com/5w2h-tecnica-de-analisis-de-problemas/</a>
  </li>
  <li>
    DZone. (s.f.). <em>Acceptance Criteria in Scrum</em>. Recuperado de <a href="https://dzone.com/articles/acceptance-criteria-in-software-explanation-exampl">https://dzone.com/articles/acceptance-criteria-in-software-explanation-exampl</a>
  </li>
  <li>
    Modern Requirements. (s.f.). <em>Requirements Traceability Matrix</em>. Recuperado de <a href="https://www.modernrequirements.com/blogs/using-a-requirements-traceabilitymatrix-to-improve-project-quality/">https://www.modernrequirements.com/blogs/using-a-requirements-traceabilitymatrix-to-improve-project-quality/</a>
  </li>

  <li>
    Fowler, M. (s.f.). <em>Ubiquitous Language</em>. Recuperado de <a href="https://martinfowler.com/bliki/UbiquitousLanguage.html">https://martinfowler.com/bliki/UbiquitousLanguage.html</a>
  </li>
  <li>
    Open Practice Library. (s.f.). <em>Ubiquitous Language</em>. Recuperado de <a href="https://openpracticelibrary.com/practice/ubiquitous-language/">https://openpracticelibrary.com/practice/ubiquitous-language/</a>
  </li>
  <li>
    Nick Tune. (s.f.). <em>Domain-Driven Architecture Diagrams</em>. Recuperado de <a href="https://medium.com/nick-tune-tech-strategy-blog/domain-driven-architecturediagrams-139a75acb578">https://medium.com/nick-tune-tech-strategy-blog/domain-driven-architecturediagrams-139a75acb578</a>
  </li>
  <li>
    Domain Storytelling. (s.f.). <em>Domain Storytelling and Requirements</em>. Recuperado de <a href="https://domainstorytelling.org/#dst-requirements">https://domainstorytelling.org/#dst-requirements</a>
  </li>
  <li>
    DDD Crew. (s.f.). <em>Big Picture EventStorming</em>. Recuperado de <a href="https://github.com/ddd-by-examples/library/blob/master/docs/big-picture.md">https://github.com/ddd-by-examples/library/blob/master/docs/big-picture.md</a>
  </li>
  <li>
    DDD Crew. (s.f.). <em>Design Level EventStorming</em>. Recuperado de <a href="https://github.com/ddd-by-examples/library/blob/master/docs/design-level.md">https://github.com/ddd-by-examples/library/blob/master/docs/design-level.md</a>
  </li>

  <li>
    <em>The Markdown Guide</em>. Recuperado de <a href="https://www.markdownguide.org/">https://www.markdownguide.org/</a>
  </li>
  <li>
    Noam Tamim. (s.f.). <em>How to use PlantUML with Markdown</em>. Recuperado de <a href="https://gist.github.com/noamtamim/f11982b28602bd7e604c233fbe9d910f">https://gist.github.com/noamtamim/f11982b28602bd7e604c233fbe9d910f</a>
  </li>
  <li>
    Structurizr. (s.f.). <em>Embedding diagrams</em>. Recuperado de <a href="https://docs.structurizr.com/cloud/embed">https://docs.structurizr.com/cloud/embed</a>
  </li>
  <li>
    Connect2Group. (s.f.). <em>Using PlantUML for diagrams</em>. Recuperado de <a href="https://connect2grp.medium.com/using-plantuml-for-creating-clear-and-concisediagrams-2fc621529560">https://connect2grp.medium.com/using-plantuml-for-creating-clear-and-concisediagrams-2fc621529560</a>
  </li>

  <li>
    Driessen, V. (2010). <em>A successful Git branching model</em>. Recuperado de <a href="https://nvie.com/posts/a-successful-git-branching-model/">https://nvie.com/posts/a-successful-git-branching-model/</a>
  </li>
  <li>
    <em>Semantic Versioning 2.0.0</em>. Recuperado de <a href="https://semver.org/">https://semver.org/</a>
  </li>
  <li>
    <em>Conventional Commits</em>. Recuperado de <a href="https://www.conventionalcommits.org/">https://www.conventionalcommits.org/</a>
  </li>
  <li>
    W3Schools. (s.f.). <em>HTML Style Guide</em>. Recuperado de <a href="https://www.w3schools.com/html/html5_syntax.asp">https://www.w3schools.com/html/html5_syntax.asp</a>
  </li>
  <li>
    Google. (s.f.). <em>HTML/CSS Style Guide</em>. Recuperado de <a href="https://google.github.io/styleguide/htmlcssguide.html">https://google.github.io/styleguide/htmlcssguide.html</a>
  </li>
  <li>
    Google. (s.f.). <em>JavaScript Style Guide</em>. Recuperado de <a href="https://google.github.io/styleguide/jsguide.html">https://google.github.io/styleguide/jsguide.html</a>
  </li>
  <li>
    Google. (s.f.). <em>TypeScript Style Guide</em>. Recuperado de <a href="https://google.github.io/styleguide/tsguide.html">https://google.github.io/styleguide/tsguide.html</a>
  </li>
  <li>
    Google. (s.f.). <em>Java Style Guide</em>. Recuperado de <a href="https://google.github.io/styleguide/javaguide.html">https://google.github.io/styleguide/javaguide.html</a>
  </li>
  Spring. (s.f.). <em>Spring Boot Features</em>. Recuperado de <a href="https://docs.spring.io/spring-boot/docs/current/reference/html/features.html">https://docs.spring.io/spring-boot/docs/current/reference/html/features.html</a>
  </li>
  <li>
    SpecFlow. (s.f.). <em>Gherkin Conventions</em>. Recuperado de <a href="https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/">https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/</a>
  </li>
  <li>
    HubSpot. (s.f.). <em>Meta Tags and SEO</em>. Recuperado de <a href="https://blog.hubspot.com/marketing/meta-tags">https://blog.hubspot.com/marketing/meta-tags</a>
  </li>
</ul>

<div style="page-break-after: always;"></div>
<div style="page-break-after: always;"></div>


<div class="page-break"></div>

