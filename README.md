Proyecto Final Power BI: Reciclaje en la Ciudad de Buenos Aires

Dashboard interactivo de Business Intelligence desarrollado como proyecto final de certificación en Data Analytics (Coderhouse). El objetivo principal es analizar el comportamiento de los Puntos Verdes y la gestión de residuos sólidos urbanos en la Ciudad Autónoma de Buenos Aires durante los años 2015 y 2016.

---

## Objetivo y Alcance:
* **Contexto:** Análisis descriptivo de la red de 86 Puntos Verdes distribuidos en todas las comunas de la CABA.
* **Métricas clave:** Volumen total y promedio de kilos recibidos por material, cantidad de visitas a los puntos, y su evolución interanual.
* **Impacto:** Proveer insumos analíticos para la toma de decisiones estratégicas y optimización de políticas públicas de higiene urbana y concientización ciudadana.

---

## Stack Tecnológico y Habilidades Aplicadas:
* **Herramienta:** Power BI (Desktop / Service).
* **Modelado de Datos:** Creación de esquema en estrella, manejo de relaciones 1:N y 1:1, y tablas calculadas (`SUMMARIZE`, `GENERATESERIES`).
* **Lenguaje DAX:** Desarrollo de medidas avanzadas para inteligencia de tiempo (`DATEADD`), cálculos de variación interanual, y parámetros interactivos.
* **Transformación de Datos (Power Query):** Limpieza de nulos, anulación de dinamización de columnas (*Unpivot*) para la unificación de pesajes de materiales, y creación de columnas condicionales y de fecha.

---

## Arquitectura y Modelo Relacional (DER)
El modelo consta de una estructura robusta integrada por tablas de dimensiones y hechos optimizadas para el filtrado cruzado:
* `PUNTO VERDE`: Catálogo de los puntos de recepción.
* `ENTREGA`: Registro histórico de pesajes por tipo de material.
* `VISITA`: Conteo y afluencia de vecinos por semana/mes.
* `DIRECCIÓN` y `COOPERATIVA`: Ubicación espacial (latitud/longitud, comunas, barrios) y gestión operativa.
* `TABLA CALENDARIO`: Dimensión temporal integrada para análisis de tendencias.

---

## Estructura del Tablero (Solapas Principales)

1. **Indicadores Generales:** Vista resumen ejecutiva con tarjetas de KPIs globales, evolución mensual de pesajes y rankings de puntos verdes y materiales.
2. **Puntos Verdes:** Mapa de distribución geográfica y proporción de puntos con y sin atención presencial.
3. **Materiales:** Análisis detallado mediante gráficos de embudo, identificación de residuos más frecuentes (Papel y Cartón) y un parámetro interactivo de porcentaje de material no reciclable (contaminado/sucio).
4. **Visitas:** Evaluación del flujo ciudadano con mapas de calor por tamaño, métricas de afluencia semanal máxima y promedio, y comparativas interanuales.

---

## Visual Previa
<img width="1162" height="660" alt="Imagen 1" src="https://github.com/user-attachments/assets/f5c36c1f-75e7-4ff5-9b90-f549845220ff" />
<img width="1169" height="661" alt="Imagen 2" src="https://github.com/user-attachments/assets/b87a47ce-ffb5-4049-8732-5f4dde47e45b" />
<img width="1168" height="657" alt="Imagen 3" src="https://github.com/user-attachments/assets/20c22395-0757-4a81-9ac3-065408ae940b" />
<img width="1163" height="647" alt="Imagen 4" src="https://github.com/user-attachments/assets/683a19e1-4ea3-4ab7-9b7d-952e58e55ed7" />

---

## Contenido del Repositorio
* `Reciclaje_CABA.pbix`: Archivo fuente del reporte de Power BI (anonimizado / optimizado).
* `screenshots/`: Carpeta con capturas de pantalla de las diferentes vistas del tablero.
