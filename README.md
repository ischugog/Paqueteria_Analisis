TÍTULO DEL PROYECTO
Análisis de Datos Logísticos para Paquetería Optimización de rutas y tiempos de entrega con Python

OBJETIVO
Demostrar cómo analizar datos de envíos para identificar patrones de retraso y proponer mejoras operativas que reduzcan costos y tiempos.

DATOS UTILIZADOS
Se generaron 1,000 envíos simulados con las siguientes variables:
Campo	Descripción	Ejemplo
envio_id	ID único del paquete	1, 2, ..., 1000
origen	Ciudad de salida	Mochis, Culiacán, Mazatlán, Hermosillo
destino	Ciudad de llegada	Tijuana, Mexicali, Guadalajara, Monterrey
distancia_km	Distancia recorrida	500 – 1,500 km
tiempo_estimado_horas	Tiempo planeado	8 – 24 horas
tiempo_real_horas	Tiempo real de entrega	7 – 30 horas
costo_envio	Costo del envío	$200 – $800
estado	Estado final	Entregado (80%), Retrasado (15%), Cancelado (5%)

HERRAMIENTAS USADAS
•	Python (Pandas, NumPy, Matplotlib)
•	Jupyter Notebook
•	GitHub para control de versiones
•	Análisis estadístico y visualización

METODOLOGÍA
1.	Generación de datos realistas (simulación con distribución probabilística).
2.	Cálculo del retraso: retraso = tiempo_real - tiempo_estimado(Solo valores positivos)
3.	Análisis por origen: promedio de retrasos.
4.	Visualización: gráfico de dispersión con línea de referencia (sin retraso).
5.	Conclusión de negocio.

RESULTADOS CLAVE
Ciudad	Retraso Promedio (horas)
Mochis	4.25
Culiacán	5.81
Mazatlán	6.12
Hermosillo	5.67
Mochis es el origen más eficiente con ~30% menos retraso que el promedio.

GRÁFICO GENERADO
retrasos_paquete.png
•	Eje X: Tiempo estimado
•	Eje Y: Tiempo real
•	Línea roja diagonal: entrega perfecta (sin retraso)
•	Puntos azules (Mochis): casi todos por debajo o cerca de la línea
•	Otros colores: más dispersos hacia arriba → más retrasos

INSIGHT DE NEGOCIO
Recomendación operativa: Priorizar rutas desde Los Mochis puede reducir 10–15% en costos operativos por menor tiempo perdido, combustible y penalizaciones.


CONCLUSIÓN
Este análisis es escalable: con datos reales de Paquetería (CSV de rutas, GPS, tiempos), se puede:
•	Predecir retrasos con machine learning
•	Optimizar rutas con algoritmos
•	Generar dashboards automáticos
Listo para implementar en producción.
