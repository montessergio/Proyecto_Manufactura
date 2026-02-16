# 📊 Análisis de Manufactura: Control de Calidad y Eficiencia

Este proyecto realiza un análisis integral de los procesos de producción, centrándose en la identificación de fallas críticas y la optimización de tiempos.

## 🛠️ Herramientas Utilizadas
* **Python (Pandas & Matplotlib):** Limpieza de datos y análisis estadístico inicial.
* **Power BI:** Creación de un Dashboard interactivo con 4 vistas principales.
* **Diagrama de Pareto:** Aplicado para identificar el 80% de los defectos.

## 📈 Contenido del Repositorio
1.  **Analisis_Proyecto_Manufactura.ipynb:** Script con el procesamiento de datos.
2.  **Proyecto_Manufactura_Graficos.pbix:** Reporte visual con indicadores de paros, defectos por máquina y tendencias.
3.  **Carpeta /export_powerbi:** Bases de datos procesadas en formato CSV.

## 💡 Insights Clave
* Se identificaron los defectos principales que afectan la línea de producción.
* El análisis de tendencias permite prever picos de fallas en turnos específicos.

🟢 SECCIÓN A: Formación del Equipo TOPS (Equipos Orientados a la Solución de Problemas) 


Nombre del Equipo: 🛠️ Ingenieros chiquitos 


👥 Estructura del Equipo: Roles y Responsabilidades 


👔 Gerente de Producción (Omar Campos): Responsable de interpretar el impacto en el throughput y asegurar el cumplimiento de las metas de entrega. Su enfoque es priorizar las acciones de mejora que impacten la productividad.


📊 Analista de Calidad (Sergio Montes / Mónica Godínez): Encargados de calcular las métricas de defectos utilizando el dataset de producción. Su función principal es ejecutar el Análisis de Pareto e identificar el defecto principal.
+2


⚙️ Ingeniero de Procesos (Karen Pérez): Responsable del diseño de soluciones técnicas y mejoras de flujo de trabajo. Su tarea es proponer mecanismos de ingeniería aplicada como Poka-Yoke.
+1


📋 Supervisor de Turno (Anahi): Encargada de validar que las propuestas sean operativamente viables en el piso de producción. Documenta las condiciones reales de operación para asegurar el éxito de la implementación.


🤝 Justificación de Multidisciplinariedad 

Para abordar la variabilidad en la planta "Manufactura Global S.A." , es vital integrar estas cuatro perspectivas:
+1

🚀 Producción: Optimiza la capacidad y el flujo para cumplir con los clientes.

🛡️ Calidad: Asegura la estabilidad estadística y que las soluciones eliminen la variabilidad.

🧪 Procesos: Traduce los datos en ingeniería aplicada y herramientas físicas concretas.

✅ Operación: Garantiza que la implementación sea realista para los operadores en todos los turnos.

📉 SECCIÓN B: Aplicación de Seis Sigma (Metodología DMAIC)
En esta sección utilizamos el ciclo de mejora para atacar la variabilidad de la planta.

1. 🎯 Definir y Medir

Métrica de Calidad Global: Calculamos el porcentaje total de unidades defectuosas de la planta (Suma de Defectos / Suma de Producción).


Análisis de Pareto: Mediante el procesamiento en Python, identificamos que el Tipo de Defecto Principal es "Dimensión fuera de especificación". Este problema representa la prioridad #1 para el equipo TOPS debido a su alto impacto en el desperdicio de material.

2. 🔍 Analizar: Caso Máquina M2
Al filtrar los datos para la Máquina M2, observamos una recurrencia crítica del defecto de dimensiones. Para encontrar la causa raíz, aplicamos la técnica de los 5 Porqués:
+1

¿Por qué las piezas de la M2 tienen dimensiones incorrectas?

Respuesta: Porque el eje de corte pierde alineación durante la operación.

¿Por qué pierde alineación el eje?

Respuesta: Porque el soporte del rodamiento presenta una vibración excesiva.

¿Por qué hay vibración excesiva?

Respuesta: Porque los tornillos de fijación se aflojan con el calor del turno.

¿Por qué se aflojan con el calor?

Respuesta: Porque no se está utilizando el torque de apriete especificado ni sellador térmico.

¿Por qué no se usa el torque correcto? (Causa Raíz)

Respuesta: Falta de un procedimiento estandarizado de ajuste y ausencia de herramientas de torque calibradas en la estación.

3. ✨ Mejorar (Lluvia de Ideas)
Tras una sesión de brainstorming, el equipo propone las siguientes soluciones:

Estandarización: Crear una Ayuda Visual (SOP) con los valores de torque específicos para la M2.

Kit de Herramientas: Proveer llaves dinamométricas (torquímetros) fijas en la estación de trabajo.

Material: Implementar el uso de arandelas de presión y sellador de roscas de alta temperatura.

4. 🛠️ Controlar
Para asegurar que la Máquina M2 se mantenga en los estándares, utilizaremos:

Gráfico de Control (SPC): Un tablero visual donde el operador registre las dimensiones críticas cada hora. Si los puntos salen de los límites, la máquina se detiene automáticamente para ajuste.
