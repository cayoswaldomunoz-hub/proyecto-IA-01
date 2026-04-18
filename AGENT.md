# 🤖 AGENT Project Overview

Este proyecto es un sistema de análisis de datos empresarial que integra múltiples especialidades de IA para transformar datos crudos en insights estratégicos y contenido persuasivo de ventas.

---

## 📂 Estructura Principal del Proyecto

```
proyecto/
├── .agent/                    # Skills (Roles de IA especializados)
├── Data/                      # Datos de entrada para análisis
│   ├── raw/                   # Datos crudos sin procesar
│   └── ventas/                # Datos de productos e inventarios
├── Informes/                  # Resultados y entregables finales
└── AGENT.md                   # Este archivo
```

---

## 🎯 Skills Disponibles en `.agent/`

Cada archivo de skill contiene un rol especializado de IA con instrucciones, metodología y mejores prácticas. La IA debe cargar el skill correspondiente según la tarea.

### 1️⃣ **analista-datos-negocio.md**
**Role:** Analista de Inteligencia de Negocios (BI) & Data Insights Specialist

**Propósito:** Transformar datos crudos en estrategia de negocio.

**Especialidades:**
- Auditoría y limpieza de datos (detectar errores, valores nulos, duplicados)
- Análisis descriptivo de KPIs (facturación, ticket promedio, margen de utilidad)
- Análisis de tendencias y series de tiempo (crecimiento vs. estancamiento)
- Generación de insights narrativos (contar la historia detrás de los números)
- Identificación de anomalías y oportunidades de optimización

**Entrada de datos:** `Data/raw/` - Datos de ventas y operaciones sin procesar

**Salida esperada:** Reportes ejecutivos, dashboards analíticos, recomendaciones estratégicas

---

### 2️⃣ **creador-contenido-ventas.md**
**Role:** Senior Direct Response Copywriter & Sales Strategist

**Propósito:** Convertir especificaciones de productos en textos persuasivos de ventas de alta conversión.

**Especialidades:**
- Identificación de "Pain Points" (puntos de dolor del cliente)
- Redacción de headlines disruptivos (thumb-stopping)
- Estructura AIDA: Attention → Interest → Desire → Action
- Copywriting emocional con urgencia y escasez
- Optimización para venta directa (Instagram, WhatsApp, e-commerce)
- CTAs claros y sin fricción

**Entrada de datos:** `Data/ventas/` - Inventario de productos y especificaciones

**Salida esperada:** Copy de ventas, mensajes promocionales, descripciones de productos persuasivas

---

### 3️⃣ **diseñador-clases-creativas.md**
**Role:** Diseñador Instruccional Creativo | Creative Instructional Designer

**Propósito:** Convertir insights y datos en contenido educativo y clases dinámicas.

**Especialidades:**
- Diseño de hooks iniciales (preguntas y datos curiosos)
- Explicaciones simplificadas con analogías del mundo real
- Diseño de actividades prácticas y creatividad
- Evaluación rápida del aprendizaje
- Adaptación de contenido para diferentes niveles

**Entrada de datos:** Resultados de análisis de datos o insights de negocios

**Salida esperada:** Planes de clase, contenido educativo, materiales de capacitación

---

## 📊 Estructura de Datos en `Data/`

### **Data/raw/**
**Propósito:** Base de datos de origen sin procesar para análisis y pruebas.

**Archivos:**
- `Datos_Ventas_Prueba_BI_Agente.csv` - Dataset de ventas para análisis BI

**Uso:** 
- El skill **analista-datos-negocio** lee y procesa estos datos
- Limpieza, validación y generación de KPIs
- Detección de patrones, tendencias y anomalías

**Formato esperado:** CSV con columnas de: Fecha, Producto, Cantidad, Precio, Región, Cliente, etc.

---

### **Data/ventas/**
**Propósito:** Datos de inventario y especificaciones de productos para crear contenido de ventas.

**Archivos:**
- `Inventario de Productos.csv` - Catálogo de productos con especificaciones

**Uso:**
- El skill **creador-contenido-ventas** transforma características técnicas en beneficios persuasivos
- Generación de copy de ventas, descripciones y mensajes promocionales
- Identificación de ángulos de venta únicos por producto

**Formato esperado:** CSV con columnas de: Nombre Producto, Descripción, Precio, Stock, Categoría, Características, etc.

---

## 📋 Estructura de Informes en `Informes/`

**Propósito:** Carpeta de destino para todos los resultados y entregables generados.

**Tipos de archivos esperados:**
- Reportes de análisis BI (.pdf, .xlsx, .md)
- Dashboards y visualizaciones de datos
- Copy de ventas y material promocional
- Planes de clase y contenido educativo
- Recomendaciones estratégicas

---

## 🔄 Flujo de Trabajo Recomendado para la IA

### **Workflow Tipo 1: Análisis → Insights**
1. Cargar skill: `analista-datos-negocio.md`
2. Leer datos desde: `Data/raw/`
3. Realizar auditoría y análisis
4. Generar informe en: `Informes/`

### **Workflow Tipo 2: Datos → Copy de Ventas**
1. Cargar skill: `creador-contenido-ventas.md`
2. Leer datos desde: `Data/ventas/`
3. Transformar especificaciones en copy persuasivo
4. Guardar contenido en: `Informes/`

### **Workflow Tipo 3: Insights → Contenido Educativo**
1. Cargar skill: `diseñador-clases-creativas.md`
2. Usar insights del análisis BI como base
3. Diseñar clase o contenido educativo
4. Guardar plan de clase en: `Informes/`

### **Workflow Integrado: Análisis Completo**
1. **Fase 1 (BI):** Analiza `Data/raw/` con skill de Analista
2. **Fase 2 (Ventas):** Crea copy de `Data/ventas/` con skill de Copywriter
3. **Fase 3 (Educación):** Diseña contenido educativo con skill de Designer
4. **Consolidación:** Genera informe ejecutivo integrando los 3 resultados en `Informes/`

---

## 🎓 Instrucciones para la IA

Cuando la IA trabaje en este proyecto:

1. **Identifica la tarea** y carga el skill correspondiente desde `.agent/`
2. **Lee los datos** desde la carpeta `Data/` apropiada
3. **Sigue la metodología** establecida en el skill seleccionado
4. **Genera resultados** de alta calidad
5. **Almacena los entregables** en la carpeta `Informes/`
6. **Documenta el proceso** para trazabilidad y mejora continua

---

**Última actualización:** 17 de abril de 2026
