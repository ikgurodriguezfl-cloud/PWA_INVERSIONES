# 🎯 Skills de IA - Catálogo Global de Capacidades

**Versión**: 1.0  
**Fecha Actualización**: 08 de Marzo 2026  
**Status**: ✅ Operativo

---

## 📋 Descripción General

Este directorio contiene la documentación completa de todos los **Skills de IA** disponibles en la metodología **AI SKILL DEVELOPMENT**.

Los **Skills** son **capacidades reutilizables** que pueden ser asignadas a uno o más agentes. Cada skill representa una unidad de conocimiento/capacidad específica.

---

## 🎭 Agentes y Sus Skills Asignados

### 🧠 **Kakashi - Orquestador**

| Skill | Descripción | Entrada | Salida |
|-------|-------------|---------|--------|
| `ticket_analyzer` | Analiza tickets y especificaciones | Ticket/SPEC.md | Requisitos técnicos |
| `architecture_designer` | Diseña arquitectura técnica | Requisitos | Diseño, diagrama |
| `requirement_validator` | Valida consistencia de requisitos | Requisitos | Reporte validación |
| `knowledge_synthesizer` | Sintetiza información en decisiones | Documentación | Decisiones doc. |

---

### 👨‍💻 **Naruto - Desarrollador Senior #1**

| Skill | Descripción | Entrada | Salida |
|-------|-------------|---------|--------|
| `react_code_generator` | Genera componentes React | Diseño | Componentes .tsx |
| `typescript_code_generator` | Genera código TypeScript | Diseño | Código .ts |
| `vite_code_generator` | Configura Vite | Config | vite.config.ts |
| `tradingview_widgets_integrator` | Integra gráficas TradingView | Diseño UI | Componentes chart |
| `broker_api_integrator` | Integra APIs de brokers | Especificación broker | Servicios conector |
| `documentation_writer` | Documenta decisiones | Código | Comentarios + Docs |
| `dependency_manager` | Gestiona dependencias | package.json | package.json actualizado |
| `code_structure_organizer` | Organiza estructura proyecto | Diseño | Árbol carpetas |

---

### 🥷 **Sasuke - Optimizador**

| Skill | Descripción | Entrada | Salida |
|-------|-------------|---------|--------|
| `code_optimizer` | Optimiza rendimiento código | Código | Código optimizado |
| `performance_analyzer` | Analiza rendimiento bajo carga | Código | Reporte (latencia, memory) |
| `security_auditor` | Audita seguridad código | Código | Reporte seguridad |
| `pattern_refactorer` | Refactoriza patrones código | Código | Código refactorizado |

---

### 🧪 **Sakura - QA Tester**

| Skill | Descripción | Entrada | Salida |
|-------|-------------|---------|--------|
| `test_case_generator` | Genera casos de prueba | Código | Tests .test.ts |
| `bug_detector` | Detecta bugs en código | Tests | Reporte bugs |
| `quality_validator` | Valida criterios calidad | Código | Reporte calidad |
| `regression_tester` | Testa regresiones | Tests | Reporte regression |

---

## 📊 Matriz Completa: Skills × Agentes

| Skill | Kakashi | Naruto | Sasuke | Sakura | Tipo | Estado |
|-------|---------|--------|--------|--------|------|--------|
| ticket_analyzer | ✅ | | | | Análisis | ✅ |
| architecture_designer | ✅ | | | | Diseño | ✅ |
| requirement_validator | ✅ | | | | Validación | ✅ |
| knowledge_synthesizer | ✅ | | | | Síntesis | ✅ |
| react_code_generator | | ✅ | | | Generación | ✅ |
| typescript_code_generator | | ✅ | | | Generación | ✅ |
| vite_code_generator | | ✅ | | | Configuración | ✅ |
| tradingview_widgets_integrator | | ✅ | | | Integración | ✅ |
| broker_api_integrator | | ✅ | | | Integración | ✅ |
| documentation_writer | | ✅ | | | Documentación | ✅ |
| dependency_manager | | ✅ | | | Gestión | ✅ |
| code_structure_organizer | | ✅ | | | Organización | ✅ |
| code_optimizer | | | ✅ | | Optimización | ✅ |
| performance_analyzer | | | ✅ | | Análisis | ✅ |
| security_auditor | | | ✅ | | Auditoría | ✅ |
| pattern_refactorer | | | ✅ | | Refactoring | ✅ |
| test_case_generator | | | | ✅ | Testing | ✅ |
| bug_detector | | | | ✅ | Testing | ✅ |
| quality_validator | | | | ✅ | Validación | ✅ |
| regression_tester | | | | ✅ | Testing | ✅ |

---

## 🔄 Skills por Fase del Desarrollo

### **FASE 2.3: Investigación**

Skills Activos:
- `ticket_analyzer` (Kakashi)
- `requirement_validator` (Kakashi)
- `knowledge_synthesizer` (Kakashi)

Objetivo: Entender requisitos y generar plan técnico

---

### **FASE 2.4: Diseño y Estructura**

Skills Activos:
- `architecture_designer` (Kakashi)
- `code_structure_organizer` (Naruto)
- `vite_code_generator` (Naruto)
- `dependency_manager` (Naruto)

Objetivo: Crear estructura base del proyecto

---

### **FASE 3: Implementación**

#### Sub-fase 3.1: Desarrollo

Skills Activos:
- `react_code_generator` (Naruto)
- `typescript_code_generator` (Naruto)
- `broker_api_integrator` (Naruto)
- `tradingview_widgets_integrator` (Naruto)
- `documentation_writer` (Naruto)

Objetivo: Implementar módulos y servicios

#### Sub-fase 3.2: Optimización (Paralela)

Skills Activos:
- `performance_analyzer` (Sasuke)
- `code_optimizer` (Sasuke)
- `security_auditor` (Sasuke)
- `pattern_refactorer` (Sasuke)

Objetivo: Optimizar y asegurar código

#### Sub-fase 3.3: Testing (Paralela)

Skills Activos:
- `test_case_generator` (Sakura)
- `bug_detector` (Sakura)
- `quality_validator` (Sakura)
- `regression_tester` (Sakura)

Objetivo: Validar y asegurar calidad

---

## 💡 Reglas para Usar Skills

### ✅ Permitido:

1. **Asignar skill ya existente a un proyecto**
   ```yaml
   # En workflow_agents.yaml del proyecto:
   naruto:
     skills:
       - react_code_generator (reaplicar en nuevo proyecto)
   ```

2. **Extender skill con parámetros específicos del proyecto**
   ```yaml
   # En workflow_agents.yaml:
   naruto:
     extended_skills:
       - broker_api_integrator:
           broker: IBKR
           apis: [market_data, order_execution, options_chain]
   ```

3. **Documentar uso del skill en proyecto**
   - Referencia en README
   - Link a skill en `ai_global/skills/`
   - Parámetros usados

### ❌ NO Permitido:

1. **Modificar skill documentación** sin validación
2. **Crear duplicados** del mismo skill con otro nombre
3. **Asignar skill a agente incorrecto** sin re-documentar
4. **Usar skill no documentado** en `ai_global/skills/`

---

## 🆕 Crear Nuevo Skill

Para agregar un nuevo skill a la metodología:

1. **Documentar en archivo .md**:
   - Propósito y descripción
   - Entrada y salida
   - Agente(s) asignado(s)
   - Ejemplos de uso

2. **Registrar en esta matriz**:
   - Agregar fila en tabla
   - Marcar agente asignado

3. **Actualizar agentes**:
   - Agregar en la documentación del agente

4. **Usar en proyecto**:
   - Referencia en `workflow_agents.yaml`

---

## 📊 Métricas de Skills

| Métrica | Valor Actual |
|---------|-------------|
| Total skills disponibles | 20 |
| Agentes con skills asignados | 4 |
| Skills por Kakashi | 4 |
| Skills por Naruto | 8 |
| Skills por Sasuke | 4 |
| Skills por Sakura | 4 |
| Proyectos usando estos skills | 0 (FASE 1) |

---

## 🔗 Referencias

- **Metodología**: [../AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../AI_SKILL_DEVELOPMENT_METHODOLOGY.md)
- **Agentes**:
  - [Kakashi Orchestrator](../agents/fic_kakashi_agent_orchestrator.md)
  - [Naruto Dev1](../agents/fic_naruto_agent_dev1.md)
  - [Sasuke Dev2](../agents/fic_sasuke_agent_dev2.md)
  - [Sakura Tester1](../agents/fic_sakura_agent_tester1.md)
- **Knowledge**: [../knowledge/README.md](../knowledge/README.md)

---

**Status**: ✅ Operativo y listo para proyectos  
**Última actualización**: 08 de Marzo 2026  
**Versión**: 1.0
