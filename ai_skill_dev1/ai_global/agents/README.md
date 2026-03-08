# 🤖 Agentes de Desarrollo AI - Índice Maestro

**Versión**: 1.0  
**Fecha Actualización**: 08 de Marzo 2026  
**Status**: ✅ Operativo

---

## 📋 Descripción General

Este directorio contiene la definición de los **4 agentes de IA autónomos** que orquestan el ciclo de desarrollo bajo la metodología **AI SKILL DEVELOPMENT**.

Estos agentes **NO son usuarios**, son **entidades autónomas** con skills específicos que actúan en secuencia coordinada durante las FASES 2 y 3 del desarrollo.

---

## 🎭 Agentes Disponibles

| Agente | Rol | Fase | Especialidad |
|--------|-----|------|-------------|
| **Kakashi** | Orquestador/Arquitecto | 2.3 - 2.4 | Análisis, diseño, investigación |
| **Naruto** | Desarrollador Senior #1 | 2.4 - 3 | Implementación, código, integración |
| **Sasuke** | Optimizador/Dev Senior #2 | 3 | Optimización, seguridad, refactoring |
| **Sakura** | QA Tester/Guardiana Calidad | 3 | Testing, validación, bugs |

---

## 🔍 Agentes Detallados

### 🧠 **fic_kakashi_agent_orchestrator**

**Archivo**: [fic_kakashi_agent_orchestrator.md](fic_kakashi_agent_orchestrator.md)

**Rol**: Analista/Arquitecto/Orquestador

**Fases**:
- FASE 2.3 (Investigación)
- FASE 2.4 (Diseño)

**Skills Principales**:
- `ticket_analyzer` - Analiza requisitos y especificaciones
- `architecture_designer` - Diseña arquitectura de soluciones
- `requirement_validator` - Valida consistencia de requerimientos
- `knowledge_synthesizer` - Sintetiza información en decisiones

**Función**:
- Investiga APIs financieras, brokers, estrategias
- Diseña arquitectura técnica del proyecto
- Genera config.yaml y workflow_agents.yaml
- Crea base de conocimiento inicial

**Deliverables**:
- Arquitectura documentada
- Diseño de skills necesarios
- Estructura de carpetas confirmada
- Plan de tickets derivados

---

### 👨‍💻 **fic_naruto_agent_dev1**

**Archivo**: [fic_naruto_agent_dev1.md](fic_naruto_agent_dev1.md)

**Rol**: Programador Senior #1

**Fases**:
- FASE 2.4 (Estructura)
- FASE 3 (Implementación)

**Skills Principales**:
- `react_code_generator` - Genera componentes React/TypeScript
- `typescript_code_generator` - Genera código TypeScript
- `vite_code_generator` - Genera configuracion Vite
- `tradingview_widgets_integrator` - Integra gráficas de TradingView
- `broker_api_integrator` - Integra APIs de brokers (IBKR, Alpaca)
- `documentation_writer` - Documenta decisiones técnicas
- `dependency_manager` - Gestiona dependencias
- `code_structure_organizer` - Organiza estructura del proyecto

**Función**:
- Implementa código Vite, React, TypeScript
- Crea servicios de brokers e indicadores técnicos
- Implementa módulos de señales de trading
- Integra APIs financieras
- Documenta con estándar FIC (EN/ES)

**Deliverables**:
- Código funcional
- Servicios base del proyecto
- Estructura de features
- Documentación inline FIC

**Estándar Obligatorio**: Todos los comentarios en código con prefijo `FIC` en inglés y español (EN/ES)

---

### 🥷 **fic_sasuke_agent_dev2**

**Archivo**: [fic_sasuke_agent_dev2.md](fic_sasuke_agent_dev2.md)

**Rol**: Optimizador/Desarrollador Senior #2

**Fase**:
- FASE 3 (Durante/Después de Naruto)

**Skills Principales**:
- `code_optimizer` - Optimiza latencia y rendimiento
- `performance_analyzer` - Analiza cuello de botellas
- `security_auditor` - Audita seguridad de código
- `pattern_refactorer` - Refactoriza patrones

**Especialidades**:
- Optimización de latencia en feeds de mercado (<100ms)
- Auditoría de seguridad de credenciales de broker
- Refactoring de lógica de gestión de riesgo

**Función**:
- Revisa latencia de datos de mercado
- Audita seguridad de API keys
- Refactoriza patrones de señales
- Optimiza rendimiento de indicadores

**Deliverables**:
- Código optimizado
- Reporte de seguridad
- Análisis de rendimiento
- Patrones refactorizados

---

### 🧪 **fic_sakura_agent_tester1**

**Archivo**: [fic_sakura_agent_tester1.md](fic_sakura_agent_tester1.md)

**Rol**: QA Tester/Guardiana de Calidad

**Fase**:
- FASE 3 (Después de Naruto/Sasuke)

**Skills Principales**:
- `test_case_generator` - Genera casos de prueba
- `bug_detector` - Detecta bugs y edge cases
- `quality_validator` - Valida criterios de calidad
- `regression_tester` - Prueba regresiones

**Especialidades**:
- Tests de estrategias de trading
- Validación de cálculos de indicadores vs TradingView
- Verificación de precisión de señales

**Función**:
- Crea tests unitarios e integración
- Valida cálculos de indicadores
- Verifica precisión de señales
- Detecta bugs y regresiones

**Deliverables**:
- Suite de tests completa
- Validación de cálculos (vs TradingView)
- Reporte de bugs
- Tests de regresión

---

## 🔄 Ciclo de Coordinación

```
┌─ FASE 2.3 (Investigación) ──────────────┐
│ Kakashi: Investiga y diseña             │
│ Deliverable: Arquitectura documentada   │
└─────────────────────────────────────────┘
                    ↓
┌─ FASE 2.4 (Estructura) ─────────────────┐
│ Naruto: Crea estructura base             │
│ Deliverable: Proyecto estructurado      │
└─────────────────────────────────────────┘
                    ↓
┌─ FASE 3 (Implementación) ───────────────┐
│ Naruto: Implementa servicios/módulos    │
│ Deliverable: Código funcional           │
└─────────────────────────────────────────┘
                    ↓
        ┌─────────────┬────────────┐
        ↓             ↓
    ┌─ Sasuke ─┐  ┌─ Sakura ─┐
    │ Optimiza │  │ Valida   │
    │ Seguridad│  │ Tests    │
    └──────────┘  └──────────┘
        ↓             ↓
        └─────────────┴────────────┐
                    ↓
            ┌─ APROBACIÓN ─┐
            │ ¿Listo?      │
            └──────────────┘
                    ↓ SÍ
            ┌─ MÓDULO LISTO ─┐
            └────────────────┘
```

**Orden**: `kakashi → naruto → (sasuke ∥ sakura) → Aprobación`

---

## 📊 Matriz de Skills por Agente

| Skill | Kakashi | Naruto | Sasuke | Sakura |
|-------|---------|--------|--------|--------|
| ticket_analyzer | ✅ | | | |
| architecture_designer | ✅ | | | |
| requirement_validator | ✅ | | | |
| knowledge_synthesizer | ✅ | | | |
| react_code_generator | | ✅ | | |
| typescript_code_generator | | ✅ | | |
| vite_code_generator | | ✅ | | |
| tradingview_widgets_integrator | | ✅ | | |
| broker_api_integrator | | ✅ | | |
| documentation_writer | | ✅ | | |
| dependency_manager | | ✅ | | |
| code_structure_organizer | | ✅ | | |
| code_optimizer | | | ✅ | |
| performance_analyzer | | | ✅ | |
| security_auditor | | | ✅ | |
| pattern_refactorer | | | ✅ | |
| test_case_generator | | | | ✅ |
| bug_detector | | | | ✅ |
| quality_validator | | | | ✅ |
| regression_tester | | | | ✅ |

---

## 🎯 Cómo Usar Este Sistema

### Para Crear un Nuevo Proyecto

1. **Consulta la arquitectura de Kakashi**
   - Lee investigación en `knowledge/local/`
   - Revisa decisiones en `knowledge/remote/`

2. **Define estructura con Naruto**
   - Crea `workflow_agents.yaml`
   - Estructura carpetas del proyecto

3. **Optimiza con Sasuke**
   - Revisa latencia de datos
   - Audita seguridad

4. **Valida con Sakura**
   - Crea tests unitarios
   - Valida indicadores

### Para Asignar un Skill a un Agente

1. Revisa el skill en `skills/README.md`
2. Verifica que el agente lo tenga en su asignación
3. Documenta uso en `workflow_agents.yaml` del proyecto

---

## 📈 Métricas de Operación

| Métrica | Valor Actual |
|---------|-------------|
| Agentes disponibles | 4 |
| Skills totales | 20 |
| Proyectos usando metodología | 0 (FASE 1) |
| Status operativo | ✅ Listo |

---

## 🔗 Referencias

- **Metodología**: [AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../AI_SKILL_DEVELOPMENT_METHODOLOGY.md)
- **Detalle Agentes**:
  - [Kakashi Orchestrator](fic_kakashi_agent_orchestrator.md)
  - [Naruto Dev1](fic_naruto_agent_dev1.md)
  - [Sasuke Dev2](fic_sasuke_agent_dev2.md)
  - [Sakura Tester1](fic_sakura_agent_tester1.md)
- **Skills**: [../skills/README.md](../skills/README.md)
- **Knowledge**: [../knowledge/README.md](../knowledge/README.md)

---

**Última actualización**: 08 de Marzo 2026  
**Version**: 1.0  
**Status**: ✅ Operativo y listo para proyectos
