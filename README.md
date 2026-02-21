📊 Análisis de Manufactura: Control de Calidad y Eficiencia Operativa
1. Descripción General

Este proyecto desarrolla un análisis integral de datos de producción enfocado en la identificación de defectos críticos, análisis de paros y propuesta de mejoras bajo metodologías Six Sigma (DMAIC) y Lean Manufacturing.

El objetivo principal es detectar las principales fuentes de variabilidad en la línea de producción, priorizar acciones correctivas y establecer mecanismos de control estadístico para estabilizar el proceso.m

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

Filtrando los datos de la Máquina M2 y aplicando la técnica de los **5 Porqués**:

1 ¿Por qué hay dimensiones fuera de especificación? Pérdida de alineación del eje de corte.
2 ¿Por qué se pierde la alineación? Vibración excesiva en el soporte del rodamiento.
3 ¿Por qué hay vibración excesiva? Aflojamiento de tornillos por efecto térmico.
4 ¿Por qué se aflojan los tornillos? Ausencia de torque especificado y sellador térmico.
5 ¿Por qué no se usa torque y sellador? Falta de procedimiento estandarizado y herramientas calibradas.

Causa raíz: Ausencia de estandarización técnica y control de torque en el montaje.

3. Propuestas de Mejora (Fase Mejorar)
El equipo generó cuatro propuestas creativas integradas:

Propuesta del Gerente de Producción (Omar)
-Mantenimiento Predictivo (PdM) Instalación de sensores de vibración y termografía en el husillo de M2.
-Rediseño del Preventivo: Cambio de limpiezas basadas en tiempo a limpiezas basadas en unidades producidas.
- Stock Crítico: Kit de "Respuesta Rápida M2" en almacén.
- Alertas de Capacidad: Si Cpk < 1.33, notificación inmediata para evaluar paro técnico.

Propuesta de la Ingeniera de Procesos (Karen)
- Poka-Yoke Digital: Guías físicas y sensores de proximidad que impiden el ciclo si la pieza no está correctamente orientada.
- Andon Dinámico 4.0: Torre de luz inteligente vinculada al script de Python (azul: preventivo próximo, naranja: tendencia a variabilidad, verde: estable).
- Kits de Set-Up "Pre-Stage": Carros de cambio rápido preconfigurados.
- Matriz de Auto-Calidad: Inspección visual cada 50 unidades con plantilla de alta resolución.
- Análisis Gemba-Digital: Cámaras de alta velocidad para detectar microparos.

Propuesta del Analista de Calidad (Sergio/Mónica)
- Gemelo Digital de Calidad: Dashboard en Power BI con un Índice de Salud de Proceso (ISP) que combina vibración, temperatura, Cpk y desgaste de herramienta.
- Bucles de Control Automatizados: Script Python que aprende "perfiles de éxito" de materia prima y ajusta alertas.
- FitBit del Operador-Mantenedor: Tablero de contribución individual que muestra el impacto de las acciones del operador en la calidad.

Propuesta de la Supervisora de Turno (Anahí)
-Entrenamiento Inmersivo "Siente la Máquina": Píldoras de conocimiento de 5 minutos al inicio de cada turno (sonidos, tacto, simulacros).
- Tablero de Guerra M2: Mapa de calor de riesgos, checklist con código de colores, fotos de "antes y después".
- Rituales de Control "La Hora Mágica": Cada hora, 3 minutos para verificar 5 piezas, registrar tendencia y limpiar un punto crítico.
- Reconocimiento y Consecuencias: Ranking de efectividad por turno y trofeo viajero para fomentar sana competencia.

4. Herramientas Lean Aplicadas
- TPM: Mantenimiento autónomo (operadores inspeccionan y limpian diariamente) ante paros por "Rotura de Herramienta".
- 5S: Estrategia de clasificación, orden y limpieza en el área de máquinas para reducir "Error del Operador".
- Poka-Yoke: Mecanismo físico (guias y sensores) para evitar piezas con dimensiones incorrectas.

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
