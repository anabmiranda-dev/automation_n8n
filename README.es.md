# 📊 Automatización de Reportes de Gestión de Tickets – Soporte L2

## 🧩 Descripción del proyecto
Este proyecto implementa una **automatización end-to-end** para la generación y distribución de **reportes de gestión de tickets del equipo de Soporte Nivel 2 (L2)**.

El workflow consolida información proveniente de herramientas Atlassian (simuladas mediante una **Mock API**), procesa métricas operativas clave y envía **reportes periódicos a los stakeholders**, permitiendo analizar volumen, tendencias y principales focos de demanda del soporte.

---

## 🎯 Objetivo
Optimizar el proceso manual de reporting mediante:
- Consolidación automática de tickets resueltos
- Estandarización de métricas operativas
- Visibilidad del volumen por **Categoría** y **Request Type**
- Identificación de **top offenders** (categorías y requests con mayor ingreso)

---

## ⚙️ Tecnologías y herramientas
- **n8n** – Workflow automation (low-code)
- **Jira (simulado con Mock API)** – Fuente de tickets
- **JSON** – Estructura de datos
- **Google Sheets (online)** – Persistencia de datos
- **Email (SMTP)** – Distribución de reportes
- **GitHub** – Versionado y documentación

---

## 🔄 Flujo del proceso (Workflow)

1. **Consulta de tickets**
   - Obtención de tickets desde Jira  
   - Para fines de demostración, se utiliza una **Mock API** que simula tickets reales

2. **Filtrado temporal**
   - Selección de tickets **resueltos** dentro de un período determinado

3. **Limpieza y normalización**
   - Eliminación de campos innecesarios
   - Normalización de categorías y request types

4. **Procesamiento de métricas**
   - Agrupación por:
     - Categoría
     - Request Type
   - Cálculo de volumen de tickets resueltos

5. **Persistencia**
   - Almacenamiento de los datos procesados en un **Google Sheet online**

6. **Distribución**
   - Envío automático de un **email con tablas embebidas**
   - Visualización de:
     - Volumen por categoría
     - Volumen por request type
     - Top offenders (mayor incoming)

---

## 📈 Métricas generadas
- Total de tickets resueltos por período
- Volumen de tickets por **Categoría**
- Volumen de tickets por **Request Type**
- Ranking de categorías con mayor demanda
- Ranking de request types con mayor ingreso

---

## 🧪 Datos de prueba
Para evitar el uso de información sensible:
- Los tickets provienen de una **Mock API**
- Los datos son completamente ficticios
- La estructura replica escenarios reales de Jira / ITSM

---

## 🖼️ Evidencias
- Export del workflow n8n (`.json`)
- Screenshots del flujo completo
- Ejemplo de Google Sheet generado
- Ejemplo de email enviado a stakeholders

---

## 🚀 Impacto del proyecto
- Reducción del esfuerzo manual de reporting
- Mejora en la visibilidad operativa del equipo L2
- Información consistente y reutilizable para toma de decisiones
- Solución escalable y adaptable a entornos productivos

---

## 🔮 Posibles mejoras
- Incorporar tickets **no resueltos** y SLA
- Agregar métricas de tiempo de resolución
- Dashboard automático (Looker / Power BI)
- Ejecución programada por cron
- Integración directa con Jira productivo

---

## 👩‍💻 Autor
**Ana M**  
Automatización · Soporte Funcional · Análisis de Datos · Low-code

