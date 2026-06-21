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
  Tras el segundo avance del proyecto, la solución ya cuenta con una Landing Page actualizada, una primera versión navegable del Frontend Web Application desplegada en Vercel y una primera versión de Backend Web Services desplegada en Railway. Esto permite validar progresivamente métricas operativas con datos persistidos, endpoints documentados en Swagger y rutas protegidas por JWT.
</p> 

<p><strong>Recomendaciones (Roadmap):</strong></p> 
<p>
  Considerando que ya se cuenta con Landing Page, Frontend Web Application y Web Services reales, se recomiendan las siguientes líneas de acción técnicas para consolidar el siguiente release:
</p> 
<ul> 
  <li> 
    <strong>Pruebas automatizadas del Backend API:</strong> Incrementar cobertura de pruebas unitarias e integración para endpoints company-scoped, permisos por rol y flujos críticos de requisición, compra, entrega y presupuesto.
  </li> 
  <li> 
    <strong>Evolución del Frontend (SPA):</strong> Completar validaciones de formularios, estados vacíos por compañía, traducciones y acciones CRUD restantes sobre datos reales.
  </li> 
  <li> 
    <strong>Modelado de la Base de Datos:</strong> Refinar constraints, índices y reglas de integridad para asegurar que los datos de usuarios, perfiles, proyectos, materiales, requisiciones, cotizaciones, órdenes de compra, inventario, entregas, proveedores, incidencias, presupuestos y mensajes se mantengan aislados por compañía.
  </li> 
  <li> 
    <strong>Integración y validación de servicios:</strong> Mantener Swagger/OpenAPI como contrato vivo, agregar smoke tests automáticos en CI/CD y documentar evidencias de Railway/Vercel por cada release.
  </li> 
</ul>

## 6.2. Video About-the-Team

| Elemento | Contenido del entregable |
| :--- | :--- |
| Nombre del archivo | `upc-pre-202610-1asi0730-12158-rqls-about-the-team-sprint-3.mp4` |
| URL Microsoft Stream | [upc-pre-202610-1asi0730-12158-rqls-about-the-team-sprint-3.mp4](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202322849_upc_edu_pe/IQDF7K3vlirDQ646tUd9EOfEAfiul9zMXnKiQsSu7htxW2k?e=jakAph&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D) |
| URL YouTube | [upc-pre-202610-1asi0730-12158-rqls-about-the-team-sprint-3.mp4](https://youtu.be/sqylf0zKJzg) |
