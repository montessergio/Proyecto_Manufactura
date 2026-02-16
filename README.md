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

## 🟢 SECCIÓN A: Formación del Equipo TOPS (Equipos Orientados a la Solución de Problemas) 


Nombre del Equipo: 🛠️ **Ingenieros chiquitos** 


👥 Estructura del Equipo: Roles y Responsabilidades 


👔 Gerente de Producción (**Omar Campos**): Responsable de interpretar el impacto en el throughput y asegurar el cumplimiento de las metas de entrega. Su enfoque es priorizar las acciones de mejora que impacten la productividad.


📊 Analista de Calidad (**Sergio Montes / Mónica Godínez**): Encargados de calcular las métricas de defectos utilizando el dataset de producción. Su función principal es ejecutar el Análisis de Pareto e identificar el defecto principal.
+2


⚙️ Ingeniero de Procesos (**Karen Pérez**): Responsable del diseño de soluciones técnicas y mejoras de flujo de trabajo. Su tarea es proponer mecanismos de ingeniería aplicada como Poka-Yoke.
+1


📋 Supervisor de Turno (**Anahi Valdez**): Encargada de validar que las propuestas sean operativamente viables en el piso de producción. Documenta las condiciones reales de operación para asegurar el éxito de la implementación.


## 🤝 Justificación de Multidisciplinariedad 

Para abordar la variabilidad en la planta "Manufactura Global S.A." , es vital integrar estas cuatro perspectivas:
+1

🚀 Producción: Optimiza la capacidad y el flujo para cumplir con los clientes.

🛡️ Calidad: Asegura la estabilidad estadística y que las soluciones eliminen la variabilidad.

🧪 Procesos: Traduce los datos en ingeniería aplicada y herramientas físicas concretas.

✅ Operación: Garantiza que la implementación sea realista para los operadores en todos los turnos.

## 📉 SECCIÓN B: Aplicación de Seis Sigma (Metodología DMAIC)
En esta sección utilizamos el ciclo de mejora para atacar la variabilidad de la planta.

1. 🎯 **Definir y Medir**

Métrica de Calidad Global: Calculamos el porcentaje total de unidades defectuosas de la planta (Suma de Defectos / Suma de Producción).


Análisis de Pareto: Mediante el procesamiento en Python, identificamos que el Tipo de Defecto Principal es "Dimensión fuera de especificación". Este problema representa la prioridad #1 para el equipo TOPS debido a su alto impacto en el desperdicio de material.

2. 🔍 **Analizar: Caso Máquina M2**
Al filtrar los datos para la Máquina M2, observamos una recurrencia crítica del defecto de dimensiones. Para encontrar la causa raíz, aplicamos la técnica de los 5 Porqués:
+1

**¿Por qué las piezas de la M2 tienen dimensiones incorrectas?**

Respuesta: Porque el eje de corte pierde alineación durante la operación.

**¿Por qué pierde alineación el eje?**

Respuesta: Porque el soporte del rodamiento presenta una vibración excesiva.

**¿Por qué hay vibración excesiva?**

Respuesta: Porque los tornillos de fijación se aflojan con el calor del turno.

**¿Por qué se aflojan con el calor?**

Respuesta: Porque no se está utilizando el torque de apriete especificado ni sellador térmico.

**¿Por qué no se usa el torque correcto? (Causa Raíz)**

Respuesta: Falta de un procedimiento estandarizado de ajuste y ausencia de herramientas de torque calibradas en la estación.

## 3. ✨ Mejorar (Lluvia de Ideas por Roles)
Tras una sesión de brainstorming multidisciplinaria, el equipo Ingenieros chiquitos propone las siguientes soluciones integrales para eliminar el defecto de "Dimensión fuera de especificación" en la Máquina M2:

👔 Desde la Gerencia de Producción (Omar Campos):


Priorización de Inversión: Autorizar la compra inmediata de los kits de herramientas para evitar que el costo por desperdicio (scrap) siga afectando el cumplimiento de entregas.


Ajuste de KPIs: Integrar el cumplimiento de los nuevos estándares de torque en los indicadores de rendimiento del turno.

📊 Desde el Análisis de Calidad (Sergio Montes / Mónica Godinez):


Validación de Materiales: Proponer y validar estadísticamente que el uso de arandelas de presión y sellador de roscas de alta temperatura reduzca la variabilidad de las dimensiones a largo plazo.


Muestreo Dirigido: Establecer un plan de inspección reforzado durante los primeros 15 días tras la implementación de las mejoras.

⚙️ Desde la Ingeniería de Procesos (Karen Pérez):


Estandarización Técnica (SOP): Diseñar la Ayuda Visual (SOP) con los valores de torque exactos, utilizando un lenguaje técnico claro y diagramas de posición para el eje de la M2.


Poka-Yoke de Herramientas: Implementar un Kit de Herramientas con llaves dinamométricas (torquímetros) pre-ajustadas al valor requerido, evitando que el operador use una fuerza incorrecta de forma manual.

📋 Desde la Supervisión de Turno (Anahi Valdez):


## Factibilidad Operativa: Asegurar que los torquímetros estén anclados o fijos en la estación para que el operador no pierda tiempo buscándolos (aplicación de orden y limpieza).


## Capacitación en Piso: Entrenar a los operadores en el uso correcto de los nuevos materiales y la lectura de la ayuda visual para garantizar una implementación realista y sostenible.

4. 🛠️ **Controlar**
Para asegurar que la Máquina M2 se mantenga en los estándares, utilizaremos:

**Gráfico de Control (SPC)**: Un tablero visual donde el operador registre las dimensiones críticas cada hora. Si los puntos salen de los límites, la máquina se detiene automáticamente para ajuste.


## 🚀 SECCIÓN C: Herramientas Lean Manufacturing
En esta sección, aplicamos pilares de Lean Manufacturing para eliminar desperdicios y robustecer el proceso productivo de la planta.

C.1. Mantenimiento Productivo Total (**TPM**): Enfoque en Mantenimiento Autónomo 🛠️
Ante los paros registrados por "Rotura de Herramienta", el equipo propone implementar el Pilar de Mantenimiento Autónomo:


**Inspección Diaria**: El operador realizará una limpieza y revisión visual de la herramienta al inicio de cada turno para detectar desgaste prematuro.


**Lubricación Estandarizada**: Se establece un programa donde el operador aplica lubricante en puntos críticos para reducir la fricción que causa las roturas.


**Detección Temprana**: Capacitar al operador para identificar sonidos o vibraciones anormales antes de que ocurra la falla catastrófica.

## C.2. Las 5S: Estrategia para reducir el "Error del Operador" 📋
Para mitigar los errores humanos detectados en el reporte, implementaremos las 5S en las estaciones de trabajo:


**Seiri (Clasificar)**: Retirar cualquier herramienta que no pertenezca a la operación de la máquina M2.


**Seiton (Ordenar)**: Utilizar tableros de sombra (shadow boards) para que cada herramienta (como el torquímetro) tenga un lugar único y marcado.


**Seiso (Limpiar)**: Mantener el área libre de virutas o aceite que puedan provocar distracciones o errores de ajuste.


**Seiketsu (Estandarizar)**: Colocar las Ayudas Visuales (SOP) diseñadas por el equipo en lugares visibles para consulta rápida.


**Shitsuke (Disciplina)**: Realizar auditorías semanales por parte de la Supervisora de Turno (Anahi) para mantener el estándar.

## C.3. Poka-Yoke: Mecanismo a prueba de errores 🛡️
Para evitar que salgan piezas con dimensiones incorrectas, proponemos un mecanismo físico de tipo "paso/no paso" (Go/No-Go gage):


**Diseño**: Un dispositivo de medición fija al final de la línea de la M2.


**Funcionamiento**: La pieza debe pasar a través de una ranura calibrada con la dimensión exacta. Si la pieza está fuera de especificación, no encajará en el dispositivo, bloqueando físicamente su avance a la siguiente etapa de empaque.


## 🎓 SECCIÓN D: Herramientas Creativas (Seis Sombreros para Pensar)
Para validar la solución propuesta (Poka-Yoke: Calibrador Paso/No-Paso), el equipo Ingenieros chiquitos aplicó la técnica de pensamiento paralelo. Todo el equipo analizó la misma solución bajo dos perspectivas críticas: los beneficios (Sombrero Amarillo) y los riesgos (Sombrero Negro).

🟡 **D.1. Análisis desde el Sombrero Amarillo (Beneficios y Valor)**
Bajo este sombrero, el equipo exploró por qué la implementación será un éxito y qué valor aporta a la planta.

**Gerente de Producción (Omar Campos)**: "Desde mi perspectiva, el beneficio principal es la recuperación del throughput. Al filtrar las piezas malas en la M2, evitamos que lleguen a empaque, eliminando el costo de re-trabajo y multas por retrasos".

**Analista de Calidad (Sergio Montes / Mónica)**: "Este sistema nos da una certeza del 100% en la segregación de producto conforme. Los datos de nuestros gráficos de control mostrarán una estabilidad que antes no teníamos".

**Ingeniero de Procesos (Karen Pérez)**: "El mayor beneficio técnico es la simplicidad. Al ser un dispositivo físico, no depende de la interpretación del operador; la pieza entra o no entra, eliminando la ambigüedad en la medición".

**Supervisor de Turno (Anahi)**: "Para el personal operativo, esto reduce el estrés y la fatiga visual. Es una herramienta rápida que permite mantener el ritmo de producción sin sacrificar la calidad".

## ⚫ D.2. Análisis desde el Sombrero Negro (Riesgos y Cautela)
Bajo este sombrero, el equipo se enfocó en los peligros, obstáculos y posibles fallas del sistema.

**Gerente de Producción (Omar Campos)**: "Mi preocupación es el costo de fabricación de estos calibradores para todas las estaciones. Debemos asegurar que el retorno de inversión por ahorro de scrap sea visible en el primer mes".

**Analista de Calidad (Sergio Montes / Mónica)**: "El riesgo crítico es la pérdida de calibración. Si el dispositivo se cae o se golpea, su dimensión interna podría cambiar, y estaríamos validando piezas erróneas sin saberlo".

**Ingeniero de Procesos (Karen Pérez)**: "Identifico un riesgo de desgaste por fricción. El contacto constante metal-metal con las piezas de la M2 desgastará el calibrador. Si no hay un plan de endurecimiento del material, el Poka-Yoke fallará".

**Supervisor de Turno (Anahi)**: "Existe el riesgo de resistencia al cambio. Si el operador siente que el calibrador 'lo detiene' para cumplir su cuota, podría intentar saltarse el paso o forzar la pieza, dañando tanto el producto como la herramienta".
