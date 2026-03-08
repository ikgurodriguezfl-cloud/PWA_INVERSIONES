# 📚 Knowledge Base - Sistema Híbrido Global

**Versión**: 1.0  
**Fecha Actualización**: 08 de Marzo 2026  
**Status**: ✅ Estructura operativa

---

## 📋 Descripción General

Este directorio contiene el **Sistema Híbrido de Gestión de Conocimiento** que funciona como fundación para todos los proyectos.

El sistema combina:
- **Local**: Conocimiento generado internamente por investigación de IA
- **Remote**: Referencias a fuentes externas oficiales y tutoriales

**Principio Fundamental**: El conocimiento se genera **ANTES** de crear tickets, para informar decisiones de implementación.

---

## 🎯 Regla de Oro - Orden de Consulta

Cuando necesitas información:

```
1. Busca en Knowledge GLOBAL (este directorio)
   ↓ (Si no encuentras)
2. Busca en Knowledge DEL PROYECTO
   ↓ (El proyecto especializa al global, NO reemplaza)
3. La información del proyecto extiende el conocimiento global
```

---

## 📂 Estructura

```
knowledge/
├── README.md                    ← Este archivo
├── local/                       # Conocimiento generado internamente
│   ├── README.md               # Índice de investigaciones
│   ├── 01_*.md                 # Investigaciones numeradas
│   ├── 02_*.md
│   ├── 03_*.md
│   ├── lesson_*.md             # Lecciones aprendidas
│   └── examples/               # Ejemplos de código
│
└── remote/                      # References externas
    ├── README.md               # Índice de referencias
    ├── *_reference.md          # Referencias documentadas
    └── *_api.md                # APIs y endpoints
```

---

## 📊 Estado Actual

| Componente | Estado | Última Actualización |
|-----------|--------|-------------------|
| **Estructura local/** | 🚧 Preparada | 2026-03-08 |
| **Estructura remote/** | 🚧 Preparada | 2026-03-08 |
| **Investigaciones** | ⏳ Pendientes | - |
| **Referencias** | ⏳ Pendientes | - |
| **FASE del Proyecto** | 🟡 FASE 1 | - |

---

## 🔄 Ciclo de Generación de Conocimiento

### Momento: FASE 2.3 (antes de tickets)

```
┌─────────────────────────────────────────────┐
│ IA (Kakashi) Analiza SPECIFICATION.md      │
└─────────────────────────────────────────────┘
                    ↓
        Identifica áreas de investigación:
        - APIs de brokers a integrar
        - Librerías de indicadores
        - Estrategias de opciones
        - Fuentes de datos mercado
                    ↓
┌─────────────────────────────────────────────┐
│ IA Genera Knowledge Local (.md)            │
└─────────────────────────────────────────────┘
                    ↓
     knowledge/local/
     ├── 01_broker_api_research.md
     ├── 02_indicators_research.md
     ├── 03_strategies_research.md
     ├── 04_data_sources_research.md
     └── 05_ai_analysis_strategy.md
                    ↓
┌─────────────────────────────────────────────┐
│ IA Genera Knowledge Remote (.md)           │
└─────────────────────────────────────────────┘
                    ↓
     knowledge/remote/
     ├── ibkr_api_reference.md
     ├── alpaca_api_reference.md
     ├── tradingview_reference.md
     ├── polygon_io_reference.md
     └── indicators_reference.md
                    ↓
┌─────────────────────────────────────────────┐
│ Kakashi Usa Knowledge en Diseño            │
└─────────────────────────────────────────────┘
                    ↓
        Referencia en:
        - config.yaml
        - workflow_agents.yaml
        - Tickets derivados
```

---

## 🎓 Tipos de Contenido

### En `local/`:

1. **Investigaciones Técnicas** (01_*_research.md)
   - Investigación de APIs de brokers
   - Comparativa de librerías de indicadores
   - Análisis de estrategias de opciones
   - Evaluación de feeds de datos

2. **Patrones y Decisiones** (02-04_*_patterns.md, *_decisions.md)
   - Patrones de integración encontrados
   - Decisiones arquitectónicas tomadas
   - Pros/contras evaluadas

3. **Lecciones Aprendidas** (lesson_*.md)
   - Problemas específicos encontrados
   - Soluciones implementadas
   - Recomendaciones para futuros proyectos

4. **Ejemplos de Código** (examples/*)
   - Snippets de conexión a brokers
   - Ejemplos de cálculos de indicadores
   - Patrones recomendados

### En `remote/`:

1. **Documentación Oficial** (*_api.md, *_reference.md)
   - APIs de IBKR, Alpaca, Polygon.io
   - Documentación oficial de TradingView
   - Especificaciones técnicas

2. **Tutoriales Externos** (*_tutorial.md)
   - Guías de estrategias de opciones
   - Análisis técnico educativo
   - Best practices de trading

3. **NotebookLM** (notebooklm_*.md)
   - Investigación profunda usando IA de Google
   - Q&A sobre proyecto
   - Síntesis de estrategias

---

## 💡 Convenciones

### Nombres de Archivos Local:

```
01_<topic>_research.md       # Investigación (numerada para orden)
02_<topic>_patterns.md       # Patrones encontrados
03_<topic>_decisions.md      # Decisión tomada
04_<topic>_strategy.md       # Estrategia de implementación
lesson_<description>.md      # Lección aprendida
```

### Nombres de Archivos Remote:

```
<source>_reference.md        # Referencia a fuente externa
<source>_api.md              # Documentación de API
<source>_tutorial.md         # Tutorial o guía
```

---

## 📈 Métricas de Conocimiento

| Métrica | Objetivo | Actual |
|---------|----------|--------|
| Investigaciones completadas | 5+ | 0 |
| Referencias externas documentadas | 10+ | 0 |
| Lecciones aprendidas al cierre proyecto | 3+ | 0 |
| Ejemplos de código disponibles | 5+ | 0 |

---

## 🔄 Cómo Usar Este Conocimiento

### Para Crear Nuevo Proyecto:

1. **Revisa knowledge/local/**
   - 01_broker_api_research.md → Entender opciones broker
   - 02_indicators_research.md → Indicadores disponibles
   - 03_strategies_research.md → Estrategias a implementar

2. **Revisa knowledge/remote/**
   - Referencias a APIs oficiales
   - Documentación de librerías
   - Tutoriales relevantes

3. **Usa en Diseño**
   - Kakashi referencia este conocimiento
   - Lo aplica en config.yaml
   - Informa decisiones de arquitectura

### Durante Desarrollo:

1. **Naruto implementa basado en conocimiento**
2. **Encuentra un problema NOT documentado?**
   - Crea `lesson_problema_encontrado.md`
   - Agrega solución
   - Referencia en ticket

3. **Al cierre de proyecto**
   - Actualiza lecciones aprendidas
   - Documen nuevos patrones encontrados

---

## 🔗 Referencias

- **Metodología**: [../AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../AI_SKILL_DEVELOPMENT_METHODOLOGY.md#section-knowledge)
- **Agentes**:
  - [Kakashi Orchestrator](../agents/fic_kakashi_agent_orchestrator.md) - Crea el conocimiento
  - [Naruto Dev1](../agents/fic_naruto_agent_dev1.md) - Usa el conocimiento
- **Subdirectorios**:
  - [local/README.md](local/README.md) - Investigaciones internas
  - [remote/README.md](remote/README.md) - Referencias externas

---

## 📋 Estado Actual

```
FASE 1 - INICIO DEL PROYECTO
  ✅ Estructura de directoriios creada
  ✅ README documentado
  ⏳ Investigaciones pendientes (Kakashi realizará en FASE 2.3)
  ⏳ Referencias externas pendientes (Kakashi documentará en FASE 2.3)
```

---

**Status**: ✅ Estructura operativa, espera investigaciones FASE 2.3  
**Última Actualización**: 08 de Marzo 2026  
**Versión**: 1.0
