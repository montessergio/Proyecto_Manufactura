### 📊 Análisis de Manufactura: Control de Calidad y Eficiencia Operativa

**1. Descripción General**

Este proyecto desarrolla un análisis integral de datos de producción enfocado en la identificación de defectos críticos, análisis de paros y propuesta de mejoras bajo metodologías Six Sigma (DMAIC) y Lean Manufacturing.

El objetivo principal es detectar las principales fuentes de variabilidad en la línea de producción, priorizar acciones correctivas y establecer mecanismos de control estadístico para estabilizar el proceso.m

**2. Herramientas Utilizadas**

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

**3. Contenido del Repositorio**

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

**SECCIÓN A: Formación del Equipo TOPS**
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

**Justificación de la Multidisciplinariedad**

La variabilidad en la planta requiere integrar distintas perspectivas:

Producción: Impacto en capacidad y flujo.

Calidad: Estabilidad estadística y reducción de variabilidad.

Procesos: Traducción de datos en soluciones técnicas.

Operación: Viabilidad práctica en turno.

**SECCIÓN B: Aplicación de Six Sigma (DMAIC)**

**1. Definir y Medir**

Métrica Global de Calidad

Se calculó el porcentaje total de unidades defectuosas:

Tasa de defectos=Total de defecto/Total de producción

Análisis de Pareto

Mediante procesamiento en Python se identificó como defecto prioritario:

“Dimensión fuera de especificación”

Este defecto concentra la mayor proporción de desperdicio y fue definido como prioridad estratégica.

**2. Analizar: Caso Máquina M2**

Filtrando los datos de la Máquina M2 y aplicando la técnica de los **5 Porqués**:

1 ¿Por qué hay dimensiones fuera de especificación? Pérdida de alineación del eje de corte.

2 ¿Por qué se pierde la alineación? Vibración excesiva en el soporte del rodamiento.

3 ¿Por qué hay vibración excesiva? Aflojamiento de tornillos por efecto térmico.

4 ¿Por qué se aflojan los tornillos? Ausencia de torque especificado y sellador térmico.

5 ¿Por qué no se usa torque y sellador? Falta de procedimiento estandarizado y herramientas calibradas.

Causa raíz: Ausencia de estandarización técnica y control de torque en el montaje.

**3. Propuestas de Mejora (Fase Mejorar)**
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

**FASE CONTROLAR: Sostenibilidad y Monitoreo Visual para Máquina M2**

Pregunta: ¿Qué métrica o tablero visual utilizarían para asegurar que la Máquina M2 se mantenga en los estándares correctos?

Nuestra Propuesta: Sistema Integrado de Control Visual "Ojo de Águila M2"
Para garantizar que la Máquina M2 se mantenga consistentemente dentro de los estándares de calidad y operación, implementaremos un sistema de control de doble capa: digital (estratégico) y físico (táctico-operativo) . Este sistema permitirá que tanto la gerencia como los operadores en piso tengan visibilidad en tiempo real del desempeño de la máquina, integrando las propuestas de todo el equipo TOPS.

1. Tablero Digital Estratégico (Power BI) – Responsabilidad del Analista de Calidad
Métrica	Fórmula / Definición	Objetivo	Frecuencia	Visualización
Índice de Salud de Proceso (ISP)	Combinación ponderada: Vibración (30%) + Temperatura (20%) + Cpk (30%) + Desgaste de herramienta (20%)	≥ 85%	Tiempo real	Semáforo grande con tendencia
Cpk (Índice de Capacidad de Proceso)	Mínimo [(LSE - Media)/3σ, (Media - LIE)/3σ]	≥ 1.33	Cada lote	Gráfico de control con meta
PPM (Partes por Millón) Defectuosas	(Unidades defectuosas / Unidades producidas) × 1,000,000	< 500 ppm	Diario	Tarjeta numérica grande
MTBF (Tiempo Medio Entre Fallas)	Tiempo total operativo / Número de paradas	En aumento	Semanal	Gráfico de tendencia
Porcentaje de Cumplimiento 5S	Auditoría diaria (0–100%)	≥ 95%	Diario	Calificación visual
🎯 Mecanismo de Alerta:

Verde: Todo OK (ISP > 85%, Cpk > 1.33)

Amarillo: Zona de precaución (ISP 70–85% o Cpk 1.0–1.33) → Notificación al supervisor

Rojo: Acción inmediata (ISP < 70% o Cpk < 1.0) → Alerta a gerencia, calidad y mantenimiento

Conexión con los roles:

Sergio (Analista): Alimenta el dashboard con datos del script Python y valida la precisión de las alertas.

Omar (Gerente): Recibe notificaciones en tiempo real y puede tomar decisiones estratégicas (como parar la línea si el ISP cae).

2. Tablero Físico Táctico "La Fortaleza Humana" – Responsabilidad del Supervisor
Ubicado junto a la Máquina M2, visible para todos los operadores y supervisores:

Elemento del Tablero	Descripción	Responsable de actualización
Semáforo de Turno	Indicador magnético del estado actual (Verde/Amarillo/Rojo)	Operador cada hora
Gráfico de Tendencia de Dimensiones	Registro manual de 5 mediciones por hora (con puntos conectados)	Operador después de "La Hora Mágica"
Checklist 5S con Fotos	Antes/Después del área y lista de verificación completada	Operador al inicio y fin del turno
Tarjeta Roja de Paro	Formato físico para reportar condiciones anormales	Cualquier operador
Ranking de Efectividad por Turno	Competencia semanal con métrica: (Unidades buenas - Tiempo de paro por error)	Supervisor (Anahí) actualiza cada tarde
Plan de Mantenimiento Autónomo	Calendario visible de tareas diarias/semanales	Operador marca al completar
Ejemplo visual del tablero físico:

text
+--------------------------------------------------+
|         🟢 TABLERO DE CONTROL M2 - TURNO A       |
+--------------------------------------------------+
| ESTADO ACTUAL:  🟢 ESTABLE  |  Cpk hoy: 1.42    |
|--------------------------------------------------|
| HORA | MEDICIÓN | TEMP | VIBRACIÓN | FIRMA OP.  |
| 06:00|    OK    | 42°C |  0.2 mm/s |   JH      |
| 07:00|    OK    | 43°C |  0.3 mm/s |   JH      |
| 08:00|    ⚠️     | 47°C |  0.6 mm/s |   JH → Av |
|--------------------------------------------------|
| TOP 5 PAROS DEL MES:                             |
| 1. Ajuste de herramienta (15 paros)              |
| 2. Limpieza de filtros (8 paros)                 |
|--------------------------------------------------|
| RANKING DE TURNOS:   🥇 Turno A (98%)            |
|                       🥈 Turno B (92%)            |
|                       🥉 Turno C (87%)            |
+--------------------------------------------------+
Conexión con los roles:

Anahí (Supervisora): Lidera la implementación, entrena a los operadores y verifica el cumplimiento.

Karen (Ingeniera de Procesos): Diseña los formatos visuales y asegura que los Poka-Yoke se reflejen en el tablero.

3. Reuniones de Revisión para Sostener el Control
Reunión	Participantes	Duración	Objetivo	Frecuencia
Reunión de Pie de Máquina	Supervisor + Operadores del turno	10 min	Revisar tablero físico, novedades del turno anterior, asignar tareas 5S	Al inicio de cada turno
Revisión DMAIC – Comité de Calidad	Equipo TOPS completo (Gerente, Analista, Ingeniero, Supervisor)	30 min	Analizar dashboard Power BI, ISP, Cpk, y decisiones de ajuste	Semanal (viernes)
Auditoría de Control Visual	Analista de Calidad + Supervisor	15 min	Verificar que tableros físicos estén actualizados y reflejen la realidad	Diario (aleatorio)
Conclusión: Un Control que Sostiene la Mejora
