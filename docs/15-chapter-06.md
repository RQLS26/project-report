# Capítulo VI: Conclusions
## 6.1. Conclusiones y recomendaciones
<p>
  Al finalizar el primer ciclo de investigación, diseño e implementación de la presencia digital de la solución <strong>Buildline</strong>, el equipo RQLS ha llegado a una serie de conclusiones clave, contrastando los resultados obtenidos con los planteamientos iniciales definidos bajo el enfoque Lean UX y el desarrollo ágil basado en Sprints.
</p> 

<p><strong>1. Validación de Problem Statements y Supuestos (Assumptions):</strong></p> 
<p>
  Inicialmente, se planteó como <em>Problem Statement</em> que las MYPES constructoras enfrentan un sobrecosto logístico estructural del 21.1% debido a procesos de abastecimiento informales (uso de WhatsApp), falta de trazabilidad entre obra y oficina, y la nula visibilidad del gasto real frente al presupuesto base (APU). A partir del Needfinding y la validación del modelo de negocio, se confirmó que existe una urgencia real por soluciones digitales que democraticen el control logístico sin requerir implementaciones de ERPs costosos.
</p> 
<p>
  Asimismo, se validó el supuesto de que los Jefes de Proyecto (segmento comprador) valoran altamente la capacidad de bloquear compras no planificadas. Sin embargo, se identificó que el éxito de la plataforma depende en gran medida de la adopción de la herramienta por parte del Ingeniero Residente en campo, lo que implica que el diseño de interfaces debe priorizar la rapidez y facilidad de uso.
</p> 

<p><strong>2. Contrastación de Hipótesis (Hypothesis Statements):</strong></p> 
<ul> 
  <li> 
    <strong>Hipótesis de Valor para Gerentes y Jefes de Proyecto:</strong> Se planteó que "Si proporcionamos paneles de control presupuestal y aprobaciones jerárquicas, los gerentes dejarán de aprobar compras 'a ciegas' y protegerán la rentabilidad". Los resultados obtenidos en la conceptualización validan esta hipótesis, siendo el control del APU el principal gatillo de interés comercial.
  </li> 
  <li> 
    <strong>Hipótesis de Valor para Residentes y Logística:</strong> Se asumió que "La digitalización de los requisitos y la validación automatizada de recepciones (Way Match) eliminarán los cuellos de botella". Esta hipótesis se mantiene validada a nivel conceptual, destacando la necesidad de adjuntar evidencia fotográfica en el flujo de abastecimiento.
  </li> 
</ul> 

<p><strong>3. Cumplimiento de Criterios de Éxito:</strong></p> 
<p>
  Durante el Sprint 1, el desarrollo de software se limitó estrictamente a la capa de presentación estática. Se logró implementar y desplegar exitosamente la Landing Page informativa de Buildline mediante GitHub Pages, cumpliendo con los criterios de aceptación definidos: navegación responsiva, presentación clara de la propuesta de valor, visualización de planes y perfiles del equipo.
</p> 
<p>
  Tras el avance del Sprint 2, la solución ya cuenta con una primera versión navegable del Frontend Web Application conectada a un mock API, por lo que las métricas operativas del sistema central (como la reducción de tiempos de cotización) podrán validarse progresivamente cuando los Web Services reales de Sprint 3 sustituyan los contratos simulados.
</p> 

<p><strong>Recomendaciones (Roadmap):</strong></p> 
<p>
  Considerando que ya se cuenta con Landing Page, Frontend Web Application y contratos de mock API, se recomiendan las siguientes líneas de acción técnicas para consolidar el segundo entregable y preparar la primera versión real de Web Services:
</p> 
<ul> 
  <li> 
    <strong>Desarrollo del Backend API:</strong> Implementar la primera versión de los Web Services utilizando <strong>.NET 8 (C#)</strong>, priorizando los endpoints requeridos por el Frontend para autenticación, usuarios, proyectos, requisiciones, cotizaciones, órdenes de compra, inventario, entregas, proveedores, incidencias, presupuestos y mensajes.
  </li> 
  <li> 
    <strong>Evolución del Frontend (SPA):</strong> Integrar progresivamente la aplicación en <strong>Vue.js</strong> con la API real, reemplazando el mock API por servicios desplegados y conservando los flujos ya implementados durante Sprint 2.
  </li> 
  <li> 
    <strong>Modelado de la Base de Datos:</strong> Implementar la base de datos relacional diseñada para usuarios, perfiles, proyectos, materiales, requisiciones, cotizaciones, órdenes de compra, inventario, entregas, proveedores, incidencias, presupuestos y mensajes, asegurando trazabilidad entre obra, logística y gerencia.
  </li> 
  <li> 
    <strong>Integración y validación de servicios:</strong> Establecer una comunicación fluida entre el frontend en Vue.js y el backend en .NET, documentar los contratos mediante Swagger/OpenAPI y realizar pruebas de integración antes del despliegue de Web Services.
  </li> 
</ul>

## 6.2. Video About-the-Team
**Enlace directo al video:** [Proyecto Buildline](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202113229_upc_edu_pe/IQB1dGiVxpVzQpCrk-JNZCiwAZ2xX-34W7a3JdRWhEfS9SU?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=omZ66Y)
