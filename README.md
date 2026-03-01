📊 Análisis de Manufactura: Control de Calidad y Eficiencia Operativa
Operational Excellence Group (OEG) - Caso de Estudio: Máquina M2
1. Descripción General
Este proyecto presenta un análisis integral de datos de producción enfocado en la reducción de variabilidad y la estabilización de procesos. A través de la integración de herramientas de análisis de datos y metodologías de mejora continua, se identifican cuellos de botella y se proponen soluciones de Ingeniería 4.0.

Objetivo: Detectar fuentes de variabilidad, priorizar acciones correctivas y establecer controles estadísticos.

Metodologías: Lean Manufacturing, Six Sigma (DMAIC), TPM y 5S.

2. Estructura del Equipo OEG (Operational Excellence Group)
El equipo opera bajo el modelo TOPS (Equipos Orientados a la Solución de Problemas):

Ingeniero de Calidad (Sergio Montes): Arquitectura de datos, métricas de defectos y Control Estadístico de Proceso (SPC).

Ingeniería de Procesos (Karen Pérez / Mónica Godínez): Diseño técnico de soluciones y estandarización (Poka-Yoke).

Gerente de Producción (Omar Campos): Evaluación de impacto en Throughput y cumplimiento de entregas.

Supervisión de Turno (Anahí Valdez): Factibilidad operativa en piso y gestión de cambio.

3. Fase de Diagnóstico (DMAIC: Definir y Medir)
Métrica Global de Calidad
Se procesó un dataset de 77,000 unidades con los siguientes hallazgos:

Tasa de Defectos: 4.29% (3,304 unidades defectuosas).

Defecto Prioritario: Mediante un Análisis de Pareto desarrollado en Python, se identificó "Dimensión fuera de especificación" como el factor crítico de desperdicio.

Análisis de Causa Raíz (Máquina M2)
Aplicando la técnica de los 5 Porqués, se determinó que la variabilidad en M2 se debe a:

Causa Raíz: Ausencia de estandarización técnica y falta de control de torque en el montaje térmico, provocando pérdida de alineación por vibración térmica.

4. Fase de Mejora y Control (Improve & Control)
Sistema Integrado "Ojo de Águila M2"
Para asegurar la sostenibilidad, se implementó una solución de doble capa:

A. Monitoreo Digital (Estratégico)
Despliegue de un Gemelo Digital de Calidad en Power BI que integra:
| KPI | Definición | Meta |
| :--- | :--- | :--- |
| ISP | Índice de Salud de Proceso (Vibración, Temp, Cpk, Desgaste) | ≥ 85% |
| Cpk | Índice de Capacidad de Proceso | ≥ 1.33 |
| PPM | Partes por Millón Defectuosas | < 500 |

B. Tablero Físico "La Fortaleza Humana" (Táctico)
Prototipo de interfaz de control visual para operadores en punto de trabajo:

Plaintext
+-------------------------------------------------------------+
|               OEG - TABLERO DE CONTROL TÁCTICO M2           |
+-------------------------------------------------------------+
| ESTADO: 🟢 ESTABLE  |  Cpk: 1.42  |  MTBF: 120 hrs          |
|-------------------------------------------------------------|
| HORA  | MEDICIÓN | TEMP. | VIBRACIÓN | FIRMA  | ACCIÓN      |
| 08:00 |    ⚠️    | 47°C  | 0.6 mm/s  | SM->AV | Ajuste Cal. |
+-------------------------------------------------------------+
5. Despliegue de Herramientas Lean Manufacturing
TPM: Mantenimiento Autónomo
Implementación de rutinas diarias para el operador (dueño del activo) para reducir paros por rotura de herramienta en un 40%.

Estrategia 5S
Reducción del "Error de Operador" mediante estandarización visual:

Seiton (Orden): Diseño de Shadow Boards para herramental crítico.

Shitsuke (Disciplina): Auditorías semanales con ranking de efectividad por turno.

Poka-Yoke de Doble Capa
Físico: Guía mecánica que impide la carga de piezas mal orientadas.

Lógico: Medición láser automática vinculada al script de Python para segregación inmediata de material no conforme.

6. Análisis de Viabilidad (Seis Sombreros)
Se evaluó la implementación del Gemelo Digital:

Sombrero Amarillo (Beneficios): Detección predictiva de fallos, reducción de scrap y empoderamiento del operador mediante datos reales.

Sombrero Negro (Riesgos): Dependencia de sensores y resistencia al cambio. Mitigación: Sistema híbrido (digital + físico) y capacitación continua.

7. Stack Tecnológico
Python: Pandas para limpieza de datos, Matplotlib para análisis exploratorio.

Power BI: Visualización de tendencias, integración de alertas y KPIs de cumplimiento.

Excel/CSV: Gestión de bases de datos para exportación dinámica.

Conclusión: Este proyecto no solo estabiliza la Máquina M2, sino que transforma la cultura organizacional hacia una manufactura inteligente basada en datos y mejora continua.
<img width="1437" height="801" alt="image" src="https://github.com/user-attachments/assets/83b63dba-ec92-46c1-8dc3-6fc4025fb8cc" />
