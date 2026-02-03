## Contexto del negocio
 **¿Qué problema intenta resolver el dataset?** Entender los factores asociados a la intención de cambio laboral de los candidatos.
**¿Qué decisión se podría tomar con estos datos?** Los resultados pueden apoyar decisiones relacionadas con estrategias de retención, optimización de procesos de reclutamiento y planificación de programas de capacitación
**¿Qué métrica es crítica?** target = intención de cambio de empleo (0/1).
## Estructura del dataset
**¿Qué representa una fila?** Un candidato
**¿Qué representa una columna?** Características del candidato
**¿Cuál es la granularidad?** Granularidad a nivel de candidato donde cada fila corresponde a un candidato y sus atributos asociados
## Calidad de los datos
**¿Hay valores nulos?**
| Columna            | Filas faltantes| Porcentaje |
|--------------------|----------------|------------|
| gender             | 4,508          | 23.53%     |
| enrolled_university| 386            | 2.01%      |
| education_level    | 460            | 2.40%      |
| major_discipline   | 2,813          | 14.68%     |
| experience         | 65             | 0.34%      |
| company_size       | 5,938          | 30.99%     |
| company_type       | 6,140          | 32.04%     |
| last_new_job       | 423            | 2.21%      |

**¿Hay duplicados?** La tabla no muestra datos duplicados
**¿Hay valores fuera de rango?** La columna company_size presenta valores no estandarizados como ‘10/49’, que requieren normalización para su análisis.
 **¿Los tipos de datos son correctos?** Los tipos de datos son coherentes con el contenido de cada columna; sin embargo, algunas variables que representan valores numéricos u ordinales se encuentran almacenadas como texto y requerirán transformación durante la etapa de limpieza
**¿Hay columnas que no se usarán?** La columna enrolled_id corresponde a un identificador técnico y no aporta valor analítico, por lo que podría ser excluida en etapas posteriores.
## Limitaciones y supuestos
**¿Qué NO miden estos datos?** El dataset no mide si el cambio laboral ocurrió realmente, sino únicamente la intención de cambio, ni incluye métricas de desempeño laboral.
**¿Hay sesgos?** El dataset esta centrado en perfiles de científicos de datos, lo que podría introducir sesgo poblacional y limita la generalización a otros roles laborales.
**¿Falta información clave?** El dataset no incluye métricas directas sobre clima organizacional, cultura empresarial o satisfacción laboral.
## Alcance del proyecto
Este proyecto se centra en análisis descriptivo y diagnóstico para identificar los factores asociados con la intención de los candidatos de cambiar de empleo. Las actividades detalladas, los entregables y los cronogramas se definen por separado en el documento de Scope of Work. No se desarrollan modelos predictivos.
