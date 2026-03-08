# 📋 Templates del Proyecto

**Versión**: 1.0  
**Fecha Creación**: 08 de Marzo 2026  
**Status**: ✅ Estructura operativa

---

## 📂 Descripción

Este directorio puede contener **templates específicos del proyecto** que extienden los templates globales.

### Ejemplos:

```
templates/
├── config.yaml.example              # Ejemplo configuración proyecto
├── feature_module_template.md       # Template para nuevo feature
├── api_integration_template.ts      # Template integración API
└── test_case_template.ts            # Template para test cases
```

---

## 🔗 Templates Globales

Los templates **base y recomendados** están en:

```
ai_skill_dev1/ai_global/templates/
├── AGENT_TEMPLATE.md
├── SKILL_TEMPLATE.md
├── TICKET_TEMPLATE.md
├── KNOWLEDGE_NOTE_TEMPLATE.md
├── SPEC_INCREMENTAL_TEMPLATE.md
├── SPECIFICATION_TEMPLATE.md
├── PROJECT_CONFIG_TEMPLATE.yaml
└── README_KNOWLEDGE_TEMPLATE.md
```

**Referencia**: [../../../../ai_global/templates/README.md](../../../../ai_global/templates/README.md)

---

## 📊 Cuándo Crear Templates Específicos

✅ **Crear template específico si**:
- Patrón se repite 3+ veces en el proyecto
- Diferente significativamente del template global
- Mejora eficiencia para este proyecto

❌ **NO crear si**:
- Existe template global que aplica
- Se usa solo 1-2 veces
- Es variación menor del global

---

## 🔗 Referencias

- **Templates Globales**: [../../../../ai_global/templates/](../../../../ai_global/templates/)
- **Methodology**: [../../../../ai_global/AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../../../../ai_global/AI_SKILL_DEVELOPMENT_METHODOLOGY.md)

---

**Status**: ✅ Estructura operativa  
**Última Actualización**: 08 de Marzo 2026  
**Versión**: 1.0
