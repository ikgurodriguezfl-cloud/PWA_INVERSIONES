# 📖 Knowledge Local - Investigaciones Internas

**Versión**: 1.0  
**Fecha Actualización**: 08 de Marzo 2026  
**Status**: ⏳ Preparada para investigaciones FASE 2.3

---

## 📋 Descripción

Este directorio contiene **investigaciones profundas generadas internamente** durante la FASE 2.3 por el agente Kakashi.

Incluye:
- 🔍 Investigaciones técnicas de APIs y librerías
- 📊 Patrones de implementación descubiertos
- 🧠 Estrategias de trading documentadas
- 💡 Decisiones arquitectónicas tomadas
- 📝 Lecciones aprendidas
- 💻 Ejemplos de código

---

## 🔄 Ciclo de Vida

```
FASE 2.3 (Por Kakashi):
1. Analiza SPECIFICATION.md
2. Investiga APIs, brokers, indicadores
3. Genera archivos 01_*.md, 02_*.md, etc.
4. Documenta decisiones

FASE 2.4+ (Por Naruto/Otros):
1. Consultan 01_*.md para fundamentar implementación
2. Durante FASE 3, descubren nuevos patrones
3. Generan lesson_*.md si encuentran soluciones no documentadas

CIERRE DE PROYECTO:
1. Aktualizan con lecciones finales
2. Agregan ejemplos de código real
```

---

## 📂 Estructura Base (Por Llenar)

### Investigaciones Principales (FASE 2.3):

```
01_broker_api_research.md            # Investigación: APIs de brokers
                                      # Contenido: IBKR vs Alpaca, pros/contras

02_indicators_research.md             # Investigación: Indicadores técnicos
                                      # Contenido: RSI, MACD, Bollinger, ATR

03_strategies_research.md             # Investigación: Estrategias de opciones
                                      # Contenido: Iron Condor, Straddle, etc.

04_data_sources_research.md           # Investigación: Fuentes de datos
                                      # Contenido: TradingView, Polygon.io, CBOE

05_ai_analysis_strategy.md            # Investigación: Estrategia IA análisis
                                      # Contenido: Combinación indicadores, confianza
```

### Ejemplos de Código (FASE 2.3+):

```
examples/
├── README.md                         # Índice de ejemplos
├── ibkr_connection_demo.tsx         # Demo: Conectar a IBKR
├── rsi_calculation_example.tsx      # Demo: Calcular RSI
├── signal_detector_example.tsx      # Demo: Detectar señales
└── options_chain_example.tsx        # Demo: Parsear opciones
```

### Lecciones Aprendidas (FASE 3+):

```
lesson_market_data_latency.md        # Problema: Latencia en feeds
lesson_broker_auth_timeout.md         # Problema: Timeout en IBKR
lesson_options_pricing_edge_case.md  # Problema: Edge case en opciones
```

---

## 📊 Convención de Contenido

### Plantilla: 01_*_research.md

```markdown
# 01_broker_api_research

**Fecha**: 2026-03-DD
**Investigador**: Claude AI (IA)
**Contexto**: Proyecto pwa_inversions_drfic

## Objetivo
[Qué se necesitaba investigar]

## Opciones Investigadas

### Opción 1: [Nombre]
- Pros: [Ventajas]
- Contras: [Desventajas]
- Código ejemplo:
```typescript
// code snippet
```

### Opción 2: [Nombre]
- Pros: [Ventajas]
- Contras: [Desventajas]

## Decisión Final
**Selección**: [Opción elegida]

**Razones**:
1. [Razón 1]
2. [Razón 2]
3. [Razón 3]

## Aplicación
- Usar en servicio: `src/services/xxx`
- Referencia en: `TKT-INVRFIC-001, TKT-INVRFIC-002`
```

### Plantilla: lesson_*.md

```markdown
# lesson_problema_específico

**Fecha**: 2026-03-DD
**Contexto**: Desarrollo TKT-INVRFIC-###
**Problema**: [Descripción corta]

## Situación
[Qué ocurrió exactamente]

## Impacto
[Cómo afectó al proyecto]

## Solución Encontrada
[Código/padrón que resolvió]

## Lecciones
- [Leccion 1]
- [Leccion 2]

## Aplicación
- Reutilizable en: [Otros módulos]
- Patrón recomendado: [Sí/No]
- Referencias: [Tickets, módulos]
```

---

## 📈 Métricas Esperadas FASE 2.3

| Investigación | Archivo | Status |
|---------------|---------|--------|
| Brokers | 01_broker_api_research.md | ⏳ Pendiente |
| Indicadores | 02_indicators_research.md | ⏳ Pendiente |
| Estrategias | 03_strategies_research.md | ⏳ Pendiente |
| Datos | 04_data_sources_research.md | ⏳ Pendiente |
| IA Analysis | 05_ai_analysis_strategy.md | ⏳ Pendiente |
| **Total** | **5 archivos** | ⏳ **Pendiente** |

---

## 🎯 Uso en Desarrollo

### Cómo Naruto Usa Esta Información:

```
TKT-INVRFIC-001: Implementar broker_connector

1. Lee: knowledge/local/01_broker_api_research.md
2. Entiende: Por qué IBKR fue elegido
3. Implementa: src/services/broker/ibkr.connector.ts
4. Referencia: En comentarios FIC
```

### Si Encuentras Problema No Documentado:

```
Durante TKT-INVRFIC-015:

Problem: "Timeout en IBKR después de 5 minutos de inactividad"

Acción:
1. Creas: lesson_broker_auth_timeout.md
2. Documentas: Solución encontrada (keepalive heartbeat)
3. Referencias: En TKT-INVRFIC-015

Resultado: Futuro conocimiento para próximos proyectos
```

---

## 🔗 Referencias

- **Knowledge Global**: [../README.md](../README.md)
- **Knowledge Remote**: [../remote/README.md](../remote/README.md)
- **Agente Creador**: [../../agents/fic_kakashi_agent_orchestrator.md](../../agents/fic_kakashi_agent_orchestrator.md)
- **Metodología**: [../../AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../../AI_SKILL_DEVELOPMENT_METHODOLOGY.md#section-knowledge-local)

---

**Status**: ⏳ A la espera de investigaciones FASE 2.3  
**Última Actualización**: 08 de Marzo 2026  
**Versión**: 1.0
