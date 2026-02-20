📊 Análisis de Manufactura: Control de Calidad y Eficiencia Operativa
1. Descripción General

Este proyecto desarrolla un análisis integral de datos de producción enfocado en la identificación de defectos críticos, análisis de paros y propuesta de mejoras bajo metodologías Six Sigma (DMAIC) y Lean Manufacturing.

El objetivo principal es detectar las principales fuentes de variabilidad en la línea de producción, priorizar acciones correctivas y establecer mecanismos de control estadístico para estabilizar el proceso.

2. Herramientas Utilizadas

Python (Pandas, Matplotlib):

Limpieza y estructuración del dataset.

Cálculo de métricas de defectos.

Análisis de Pareto.

Análisis exploratorio de datos.

Power BI:

Construcción de dashboard interactivo.

Visualización de defectos por máquina.

Tendencias por turno.

Indicadores clave de desempeño (KPIs).

3. Contenido del Repositorio

Analisis_Proyecto_Manufactura.ipynb
Notebook con el procesamiento de datos, análisis estadístico y generación de gráficos iniciales.

Proyecto_Manufactura_Graficos.pbix
Dashboard interactivo que incluye:

Indicadores de defectos.

Análisis de paros.

Tendencias temporales.

Identificación de máquina crítica.

/export_powerbi
Bases de datos procesadas en formato CSV listas para visualización.

SECCIÓN A: Formación del Equipo TOPS
(Equipos Orientados a la Solución de Problemas)

Nombre del Equipo: 🛠️ Ingenieros chiquitos

Estructura del Equipo y Responsabilidades

👔 Gerente de Producción (Omar Campos)
Responsable de evaluar el impacto en el throughput y priorizar acciones con efecto directo en productividad y cumplimiento de entregas.

📊 Analista de Calidad (Sergio Montes / Mónica Godínez)
Encargados del procesamiento del dataset, cálculo de métricas de defectos y ejecución del Análisis de Pareto para identificar el defecto prioritario.

⚙️ Ingeniero de Procesos (Karen Pérez)
Responsable del diseño técnico de soluciones, estandarización de procesos y propuesta de mecanismos de ingeniería aplicada como Poka-Yoke.

📋 Supervisor de Turno (Anahi Valdez)
Encargada de validar la factibilidad operativa en piso de producción y asegurar la correcta implementación de las mejoras.

Justificación de la Multidisciplinariedad

La variabilidad en la planta requiere integrar distintas perspectivas:

Producción: Impacto en capacidad y flujo.

Calidad: Estabilidad estadística y reducción de variabilidad.

Procesos: Traducción de datos en soluciones técnicas.

Operación: Viabilidad práctica en turno.

SECCIÓN B: Aplicación de Six Sigma (DMAIC)
1. Definir y Medir
Métrica Global de Calidad

Se calculó el porcentaje total de unidades defectuosas:

Tasa de defectos
=
Total de defectos
Total de producci
o
ˊ
n
Tasa de defectos=
Total de producci
o
ˊ
n
Total de defectos
	​

Análisis de Pareto

Mediante procesamiento en Python se identificó como defecto prioritario:

“Dimensión fuera de especificación”

Este defecto concentra la mayor proporción de desperdicio y fue definido como prioridad estratégica.

2. Analizar: Caso Máquina M2

Al segmentar el análisis por máquina, se identificó que la Máquina M2 presenta la mayor incidencia del defecto dimensional.

Análisis de Causa Raíz – Técnica 5 Porqués

Problema: Dimensiones fuera de especificación en M2.

Secuencia lógica:

Pérdida de alineación del eje de corte.

Vibración excesiva en soporte del rodamiento.

Aflojamiento de tornillos por efecto térmico.

Ausencia de torque especificado y sellador térmico.

Falta de procedimiento estandarizado y herramientas calibradas.

Causa raíz identificada:
Ausencia de estandarización técnica y control de torque.

3. Mejorar
Acciones Propuestas por Rol

👔 Producción

Priorización de inversión en herramientas de torque.

Integración del cumplimiento de estándares en KPIs de turno.

📊 Calidad

Validación estadística del uso de arandelas de presión y sellador térmico.

Plan de inspección reforzado post-implementación.

⚙️ Procesos

Diseño de SOP con valores de torque definidos.

Implementación de torquímetros pre-ajustados.

📋 Supervisión

Asegurar disponibilidad física de herramientas.

Capacitación operativa en piso.

4. Controlar

Se propone implementar:

Gráficos de Control (SPC) para dimensiones críticas.

Registro horario de mediciones.

Acción correctiva inmediata ante puntos fuera de límites.

SECCIÓN C: Aplicación de Lean Manufacturing
C.1 Mantenimiento Productivo Total (TPM)

Enfoque en Mantenimiento Autónomo:

Inspección visual diaria.

Lubricación estandarizada.

Detección temprana de vibraciones anormales.

C.2 Implementación de 5S

Clasificación de herramientas.

Orden mediante tableros sombra.

Limpieza sistemática.

Estandarización visual.

Auditorías periódicas.

C.3 Poka-Yoke

Diseño de calibrador Paso/No-Paso:

Dispositivo físico fijo al final de la línea.

Bloqueo automático de piezas fuera de especificación.

Eliminación de ambigüedad en medición manual.

SECCIÓN D: Evaluación Crítica de la Solución

Aplicación de técnica de análisis paralelo:

Beneficios esperados

Reducción de scrap.

Estabilidad estadística.

Simplicidad operativa.

Disminución de retrabajo.

Riesgos identificados

Pérdida de calibración del dispositivo.

Desgaste por fricción.

Resistencia al cambio.

Retorno de inversión inicial.

Conclusión

El análisis permitió:

Identificar la máquina crítica.

Priorizar defecto principal.

Determinar causa raíz técnica.

Diseñar soluciones integradas bajo enfoque DMAIC y Lean.

Proponer mecanismos de control estadístico sostenibles.

Este proyecto demuestra la integración de análisis de datos, mejora de procesos y diseño de soluciones técnicas aplicadas a entornos de manufactura.
