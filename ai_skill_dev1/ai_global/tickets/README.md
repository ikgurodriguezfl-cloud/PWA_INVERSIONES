# 🎫 Tickets Globales - Control de Cambios

**Versión**: 1.0  
**Fecha Actualización**: 08 de Marzo 2026  
**Status**: ✅ Estructura operativa

---

## 📋 Descripción

Este directorio contiene la **definición y control de tickets globales** que pueden ser compartidos entre múltiples proyectos o afectar la política general de desarrollo.

Los **Tickets Locales** (por proyecto) residen en `projects/pwa/<PROJECT>/src/ai_work_flow/tickets/`

---

## 🎯 Convenciones de Tickets

### Nomenclatura:

| Tipo | Formato | Ejemplo | Alcance |
|------|---------|---------|---------|
| **Global** | `TKT-GLOBAL-###` | `TKT-GLOBAL-001` | Afecta metodología/infraestructura |
| **Proyecto** | `TKT-<PROJ>-###` | `TKT-INVRFIC-001` | Específico de proyecto pwa_inversions_drfic |

---

## 📊 Estados de Ticket

```
Open (🟢 Abierto)
    ↓
In Progress (🟡 En Desarrollo)
    ↓
Review (🟠 En Revisión)
    ↓
Closed (✅ Completado)
```

### Reglas de Transición:

- **Open → In Progress**: Cuando comienza trabajo
- **In Progress → Review**: Cuando código está completado
- **Review → Closed**: SOLO con evidencia de prueba

---

## 📋 Política de Cierre (Obligatoria)

**REGLA CRÍTICA**: Un ticket SOLO puede cerrarse con evidencia de prueba.

### Evidencia Mínima Requerida:

✅ **Todos los Tickets**:
- [ ] Fecha de cierre
- [ ] Responsable que valida
- [ ] Estado: ✅ APROBADO o ❌ REQUIERE FIXES

✅ **Tickets de Código**:
- [ ] Tests ejecutados (resultado: PASS/FAIL)
- [ ] Commit hash
- [ ] Cambios de archivos listados

✅ **Tickets de Indicadores Financieros**:
- [ ] Validación vs TradingView o referencia
- [ ] Precisión: ±X%
- [ ] Datos históricos testeados

✅ **Tickets de Trading**:
- [ ] Señales testeadas con datos históricos
- [ ] Win rate calculado
- [ ] Paper trading validación (si aplica)

### Prohibido ❌:

- ❌ Cerrar por "código terminado" SIN validación
- ❌ Cerrar sin evidencia de pruebas
- ❌ Cerrar con tests fallidos
- ❌ Cerrar sin que Sakura tenga validada calidad

---

## 📊 Estructura de Ticket

### Plantilla Estándar:

```markdown
# TKT-GLOBAL-###: <Título>

**Metadata**:
- **Tipo**: Mejora / Corrección / Investigación / Infraestructura
- **Prioridad**: Alta / Media / Baja
- **Estado**: 🟢 Open / 🟡 In Progress / 🟠 Review / ✅ Closed
- **Creado**: YYYY-MM-DD
- **Relacionado**: TKT-GLOBAL-###, TKT-INVRFIC-###

---

## Descripción
[Qué necesita hacerse y por qué]

## Archivos Afectados
[Qué carpetas/archivos se modifican]

## Plan de Implementación
[Cómo se va a resolver]

## Criterios de Aceptación
- [ ] Criterio 1
- [ ] Criterio 2
- [ ] Criterio 3

---

## Cierre

**Fecha Cierre**: YYYY-MM-DD  
**Responsable**: Nombre  
**Status**: ✅ APROBADO

**Evidencia**:
- Tests: PASSED ✅
- Validación: [Descripción]
- Referencias: [Links/commits]
```

---

## 📂 Estructura (Por Llenar)

### Ejemplos de Tickets Globales:

```
TKT-GLOBAL-001.md              # Crear estructura inicial (FASE 1)
TKT-GLOBAL-002.md              # Definir estándares FIC (FASE 1)
TKT-GLOBAL-003.md              # Setup de CI/CD (FASE 1)
...
```

---

## 📈 Métricas de Tickets

| Métrica | Valor Actual |
|---------|-------------|
| Total tickets globales | 0 |
| Abiertos | 0 |
| En progreso | 0 |
| En revisión | 0 |
| Cerrados | 0 |
| Tasa cierre | N/A |

---

## 🔄 Ciclo de Vida de Ticket

```
CREACIÓN (Alguien identifica necesidad):
  ├─ Título claro
  ├─ Descripción completa
  └─ Criterios de aceptación
        ↓
  Ticket entra Estado: Open 🟢
        ↓
DESARROLLO:
  ├─ Alguien se asigna
  ├─ Actualiza estado: In Progress 🟡
  └─ Implementa cambios
        ↓
  Trabajo completado
        ↓
VALIDACIÓN:
  ├─ Actualiza estado: Review 🟠
  ├─ Prepara evidencia de pruebas
  └─ Solicita aprobación
        ↓
APROBACIÓN:
  ├─ Reviewer valida evidencia
  ├─ Marca criterios ✅
  └─ Aprueba SOLO si todo OK
        ↓
CIERRE:
  ├─ Actualiza estado: Closed ✅
  ├─ Documenta fecha
  └─ Ticket archivado
```

---

## 🎓 Ejemplo: Ticket Global

```markdown
# TKT-GLOBAL-001: Crear Estructura Inicial de FASE 1

**Metadata**:
- **Tipo**: Infraestructura
- **Prioridad**: Alta
- **Estado**: ✅ Closed
- **Creado**: 2026-03-08

---

## Descripción
Crear estructura global de agentes, skills, knowledge y tickets
para que el proyecto esté listo para FASE 2.

## Archivos Afectados
```
ai_skill_dev1/ai_global/
├── agents/
│   ├── README.md
│   ├── fic_kakashi_agent_orchestrator.md
│   ├── fic_naruto_agent_dev1.md
│   ├── fic_sasuke_agent_dev2.md
│   └── fic_sakura_agent_tester1.md
├── skills/README.md
├── knowledge/
│   ├── README.md
│   ├── local/README.md
│   └── remote/README.md
└── tickets/README.md (este archivo)
```

## Plan de Implementación
1. Crear 5 archivos de agentes (con descripción completa)
2. Crear README.md de skills (con matriz de skills)
3. Crear README.md de knowledge general + local + remote
4. Crear README.md de tickets (políticas de cierre)

## Criterios de Aceptación
- [ ] 5 agentes documentados correctamente
- [ ] Matriz de skills completa
- [ ] Política de cierre de tickets clarificada
- [ ] Todos archivos con status ✅ Operativo

---

## Cierre

**Fecha Cierre**: 2026-03-08  
**Responsable**: Sistema IA  
**Status**: ✅ COMPLETADO

**Evidencia**:
- Agentes: 5 archivos .md creados ✅
- Skills: README.md con matriz 20 skills ✅
- Knowledge: 3 README.md (raíz, local, remote) ✅
- Tickets: Este README.md ✅
- Validación: Estructura lista para FASE 2.3 ✅
```

---

## 🔗 Referencias

- **Metodología**: [../AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../AI_SKILL_DEVELOPMENT_METHODOLOGY.md#section-tickets)
- **Agentes**: [../agents/README.md](../agents/README.md)
- **Skills**: [../skills/README.md](../skills/README.md)
- **Knowledge**: [../knowledge/README.md](../knowledge/README.md)

---

**Status**: ✅ Estructura operativa  
**Última Actualización**: 08 de Marzo 2026  
**Versión**: 1.0
