# 🎫 Tickets del Proyecto

**Versión**: 1.0  
**Fecha Creación**: 08 de Marzo 2026  
**Status**: ✅ Estructura operativa

---

## 📋 Descripción

Control de **tickets internos de desarrollo** del proyecto pwa_inversions_e2.

Incluye:
- 🎫 Tareas de implementación
- 🐛 Bugs reportados
- 🔧 Mejoras solicitadas
- 📚 Documentación necesaria

---

## 📊 Nomenclatura

```
TKT-INVRFIC-001.md        # Ticket proyecton inversiones
TKT-INVRFIC-002.md
TKT-INVRFIC-###.md
```

**Referencia Global**: `TKT-GLOBAL-###.md` (en `ai_global/tickets/`)

---

## 🔄 Ciclo de Vida

```
1. CREAR: Identificar necesidad
   ↓
2. INICIAR: Asignar a agente, estado Open → In Progress
   ↓
3. DESARROLLAR: Agente trabaja
   ↓
4. VALIDAR: Cambiar a Review, preparar evidencia
   ↓
5. APROBAR: Sakura valida, estado Review → Closed
   ↓
6. CERRAR: Solo con evidencia ✅
```

---

## 📝 Estructura Básica

```markdown
# TKT-INVRFIC-001: Título descriptivo

**Metadata**:
- **Tipo**: Implementación / Corrección / Testing / Investigación
- **Prioridad**: Alta / Media / Baja
- **Estado**: 🟢 Open
- **Creado**: 2026-03-DD
- **Asignado a**: Naruto / Sasuke / Sakura / Kakashi

---

## Descripción
...

## Criterios de Aceptación
- [ ] Criterio 1
- [ ] Criterio 2

---

## Cierre
Fecha: [completar]
Status: ✅ APROBADO / 🔴 REQUIERE FIXES
Evidencia: [tests, validaciones, commits]
```

---

## 📊 Estados de Tickets

| Estado | Símbolo | Significado |
|--------|---------|------------|
| Open | 🟢 | Recién creado, no comenzó |
| In Progress | 🟡 | Alguien está trabajando |
| Review | 🟠 | Completado, esperando validación |
| Closed | ✅ | TERMINADO Y APROBADO |

---

## 🎯 Cómo Crear Primer Ticket

1. **Ve a esta carpeta**: `projects/pwa/pwa_inversions_e2/src/ai_work_flow/tickets/`
2. **Crea archivo**: `TKT-INVRFIC-001.md`
3. **Copia estructura** de arriba
4. **Define metadata y criterios**
5. **Comienza desarrollo**

---

## 🚫 Regla Crítica: Política de Cierre

**NUNCA cerrar un ticket sin**:
- ✅ Evidencia de validación (tests PASSED)
- ✅ Fecha creación y cierre
- ✅ Status de aprobación
- ✅ Referencias (commits, validaciones)

**Prohibido**:
- ❌ "Terminado" sin validación
- ❌ Cerrar con tests fallidos
- ❌ Sin aprobación de Sakura (si aplica)

---

## 📊 Tickets Esperados (Derivados FASE 2.3)

Kakashi generará ~10-15 tickets como:

```
TKT-INVRFIC-001: Implementar Broker Connector IBKR
TKT-INVRFIC-002: Implementar Market Data Feed
TKT-INVRFIC-003: Implementar RSI Indicator
TKT-INVRFIC-004: Implementar MACD Indicator
TKT-INVRFIC-005: Implementar Signal Detector
TKT-INVRFIC-006: Implementar Dashboard Principal
...y más
```

---

## 🔗 Referencias

- **Tickets Globales**: [../../../../ai_global/tickets/README.md](../../../../ai_global/tickets/README.md)
- **Workflow**: [../development/workflow_agents.yaml](../development/workflow_agents.yaml)
- **Methodology**: [../../../../ai_global/AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../../../../ai_global/AI_SKILL_DEVELOPMENT_METHODOLOGY.md#section-tickets)

---

**Status**: ✅ Estructura operativa, a espera de tickets FASE 2.3  
**Última Actualización**: 08 de Marzo 2026  
**Versión**: 1.0
