# 📚 Knowledge Base del Proyecto

**Versión**: 1.0  
**Fecha Creación**: 08 de Marzo 2026  
**Status**: ✅ Estructura operativa

---

## 📋 Descripción

Knowledge base **específica del proyecto** que especializa el conocimiento global.

**Estructura Híbrida**:
- **Local**: Investigaciones específicas del proyecto
- **Remote**: Referencias externas relevantes al proyecto

---

## 🔄 Relación con Knowledge Global

```
Priority de Consulta:

1. Knowledge PROYECTO (específico)
   └─ Si encontramos, usamos
   
2. Knowledge GLOBAL (base)
   └─ Si no hay específico
   
3. Nueva investigación
   └─ Si no existe en ninguno lado
```

**Regla**: Proyecto **especializa** global, no reemplaza.

---

## 📂 Estructura

```
knowledge/
├── README.md (este archivo)
├── local/
│   ├── README.md
│   ├── 01_proyecto_decisions.md
│   ├── 02_proyecto_patterns.md
│   └── lesson_*.md
└── remote/
    ├── README.md
    ├── proyecto_references.md
    └── notebooklm_proyecto.md
```

---

## 📊 Contenido Esperado (FASE 2.3+)

### Local

```
01_proyecto_specific_decisions.md   # Decisiones específicas del proyecto
02_proyecto_architecture_patterns.md # Patrones encontrados
03_proyecto_integration_notes.md     # Notas de integración
lesson_problema_1.md                 # Lecciones aprendidas
lesson_problema_2.md
```

### Remote

```
proyecto_broker_integration_ref.md   # Referencia integración broker
proyecto_indicators_validation.md     # Validación indicadores
notebooklm_proyecto_research.md      # Investigación IA del proyecto
```

---

## 🔗 Referencias

- **Knowledge Global**: [../../../../ai_global/knowledge/README.md](../../../../ai_global/knowledge/README.md)
- **Local Details**: [local/README.md](local/README.md)
- **Remote Details**: [remote/README.md](remote/README.md)
- **Methodology**: [../../../../ai_global/AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../../../../ai_global/AI_SKILL_DEVELOPMENT_METHODOLOGY.md)

---

**Status**: ✅ Estructura operativa, a espera de población FASE 2.3+  
**Última Actualización**: 08 de Marzo 2026  
**Versión**: 1.0
