# 🔗 Knowledge Remote - Referencias Externas

**Versión**: 1.0  
**Fecha Actualización**: 08 de Marzo 2026  
**Status**: ⏳ Preparada para referencias FASE 2.3

---

## 📋 Descripción

Este directorio contiene **referencias y enlaces a fuentes externas** de conocimiento documentadas por Kakashi.

Incluye:
- 🔗 URLs a documentación oficial de APIs
- 📚 Tutoriales de estrategias de trading
- 🌐 Estándares technológicos
- ☁️ Herramientas cloud de investigación (NotebookLM)
- 📊 Recursos educativos financieros

---

## 🎯 Tipos de Referencias

### 1. **APIs Oficiales** (*_api.md, *_reference.md)

Documentación autorizada de brokers y proveedores:
- Interactive Brokers TWS API
- Alpaca Trading API
- TradingView Lightweight Charts
- Polygon.io Market Data
- CBOE Options Data

### 2. **Tutoriales y Guías** (*_tutorial.md, *_guide.md)

Material educativo:
- Estrategias de opciones (Iron Condor, Straddle, etc.)
- Análisis técnico (RSI, MACD, Bollinger)
- Trading algorítmico best practices

### 3. **Herramientas IA** (notebooklm_*.md)

Investigación profunda usando IA:
- Google NotebookLM para análisis de documentos
- Q&A sobre proyecto de inversiones
- Síntesis de estrategias complejas

### 4. **Estándares y Regulaciones** (*_standard.md, *_regulatory.md)

Requisitos técnicos y legal:
- FINRA requirements
- SEC guidelines
- Data protection standards

---

## 💡 Estructura de Referencia

### Plantilla Estándar:

```markdown
# <source>_reference.md

## [Título de la Fuente]

**Tipo**: Documentación Oficial / Tutorial / API Reference / Otro  
**URL**: <enlace directo>  
**Fecha Creación**: YYYY-MM-DD  
**Última Verificación**: YYYY-MM-DD  
**Acceso**: Público / Requiere Cuenta / Requiere API Key  

### Resumen
[Breve descripción y relevancia para el proyecto]

### Puntos Clave
- Concepto/Endpoint importante 1
- Concepto/Endpoint importante 2
- Limitación o rate limit relevante

### Directamente Aplicable
[Cómo se usa en pwa_inversions_drfic]

### Relacionado Con
- Knowledge local: 01_*.md
- Tickets: TKT-INVRFIC-001, TKT-INVRFIC-005
```

---

## 📂 Estructura Base (Por Llenar)

### APIs Principales (FASE 2.3):

```
ibkr_api_reference.md                # Ref: Interactive Brokers API
alpaca_api_reference.md              # Ref: Alpaca Trading API
tradingview_widgets_reference.md     # Ref: TradingView Lightweight Charts
polygon_io_reference.md              # Ref: Polygon.io Market Data
cboe_options_reference.md            # Ref: CBOE Options Data
```

### Tutoriales y Guías (FASE 2.3):

```
options_strategies_guide.md          # Guía: Estrategias de opciones
technical_analysis_reference.md      # Ref: Análisis técnico
trading_risk_management.md           # Guía: Risk management
```

### Herramientas IA (FASE 2.3):

```
notebooklm_main_research.md          # NotebookLM: Investigación profunda
```

### Estándares (Opcional):

```
finra_requirements.md                # Requerimientos FINRA
sec_guidelines.md                    # SEC Guidelines
```

---

## 🎓 Ejemplo: Referencia a IBKR

```markdown
# ibkr_api_reference.md

## Interactive Brokers TWS API Documentation

**Tipo**: Documentación Oficial Interactive Brokers  
**URL**: https://interactivebrokers.github.io/tws-api/  
**Fecha Creación**: 2026-03-03  
**Última Verificación**: 2026-03-03  
**Acceso**: Público

### Resumen
Documentación oficial de Interactive Brokers para conexión, obtención de datos
de mercado en tiempo real y ejecución de órdenes.

### Puntos Clave
- **reqMktData()**: Suscribirse a precios en tiempo real
- **placeOrder()**: Enviar órdenes de compra/venta
- **reqOptionChain()**: Obtener cadena de opciones (strikes, expiraciones)
- **reqHistoricalData()**: Obtener velas OHLCV históricas
- **Rate limit**: 50 solicitudes simultáneas (cuenta básica)

### Directamente Aplicable
- Servicio: `src/services/broker/ibkr.connector.ts`
- Módulo: `src/features/broker-connect/`
- Para: Conexión, data streaming, order execution

### Relacionado Con
- Knowledge local: `01_broker_api_research.md` (recomendación de IBKR)
- Tickets: `TKT-INVRFIC-001` (Broker Connection), `TKT-INVRFIC-007` (Options Chain)
```

---

## 🎓 Ejemplo: NotebookLM Research

```markdown
# notebooklm_main_research.md

## NotebookLM: Investigación Profunda Proyecto pwa_inversions_drfic

**Tipo**: Herramienta IA (Google AI)  
**URL**: https://notebooklm.google.com/notebook/<ID_del_notebook>  
**Fecha Creación**: 2026-03-03  
**Última Actualización**: 2026-03-03  
**Acceso**: Requiere cuenta de Google (usuario_autenticado@email.com)

### Descripción
Notebook de investigación con análisis profundo usando IA de Google.
Contiene análisis de especificación, APIs financieras, estrategias de trading.

### Fuentes Subidas
- ✅ SPECIFICATION.md (especificación completa)
- ✅ Knowledge local (01_*.md a 05_*.md)
- ✅ Documentación IBKR API
- ✅ Documentación TradingView
- ✅ Referencias de estrategias opciones

### Capacidades Disponibles
- 💬 Responde preguntas sobre el proyecto
- 📊 Genera resúmenes de estrategias
- 🔍 Encuentra inconsistencias
- 💡 Sugiere mejoras en lógica de señales

### Preguntas Clave Respondidas
1. "¿Qué indicadores combinar para máxima confiabilidad?"
   → Respuesta: RSI(14) + MACD(12,26,9) + Bollinger(20,2)

2. "¿Cómo detectar posicionamiento institucional?"
   → Respuesta: Analizar Open Interest + Volume en opciones

### Cómo Usar
1. Acceder con cuenta Google autorizada
2. Hacer preguntas durante desarrollo
3. Copiar insights importantes a este archivo
4. Actualizar con hallazgos finales

### Relacionado Con
- Proyecto: pwa_inversions_drfic
- Knowledge local: todos los 01_*.md a 05_*.md
- Todos los tickets (contexto general)
```

---

## 📊 Referencias Esperadas FASE 2.3

| Tipo | Archivo | URL | Status |
|------|---------|-----|--------|
| API | ibkr_api_reference.md | [IBKR Docs](https://interactivebrokers.github.io/tws-api/) | ⏳ Pendiente |
| API | alpaca_api_reference.md | [Alpaca Docs](https://docs.alpaca.markets/) | ⏳ Pendiente |
| Ref | tradingview_widgets_reference.md | [TradingView Docs](https://tradingview.github.io/lightweight-charts/) | ⏳ Pendiente |
| API | polygon_io_reference.md | [Polygon.io API](https://polygon.io/docs/stocks) | ⏳ Pendiente |
| Guía | options_strategies_guide.md | [Tutorial] | ⏳ Pendiente |
| IA | notebooklm_main_research.md | [NotebookLM] | ⏳ Pendiente |

---

## 🔄 Cómo Usar Referencias

### Durante Implementación:

```
TKT-INVRFIC-001: Implementar broker_connector

1. Lee: knowledge/remote/ibkr_api_reference.md
2. Consulta: Métodos API específicos
3. Implementa: Basándose en documentación oficial
4. Valida: Contra referencia
```

### Para Investigación Profunda:

```
Pregunta: "¿Es mejor usar RSI + MACD o RSI + Bollinger?"

1. Accede: notebooklm_main_research.md
2. Abre: URL del NotebookLM
3. Pregunta: "Compare combinaciones de indicadores"
4. Obtiene: Análisis con IA de múltiples fuentes
5. Documenta: Respuesta en knowledge/local/
```

---

## 🔗 Referencias

- **Knowledge Global**: [../README.md](../README.md)
- **Knowledge Local**: [../local/README.md](../local/README.md)
- **Agente Creador**: [../../agents/fic_kakashi_agent_orchestrator.md](../../agents/fic_kakashi_agent_orchestrator.md)
- **Metodología**: [../../AI_SKILL_DEVELOPMENT_METHODOLOGY.md](../../AI_SKILL_DEVELOPMENT_METHODOLOGY.md#section-knowledge-remote)

---

**Status**: ⏳ A la espera de referencias FASE 2.3  
**Última Actualización**: 08 de Marzo 2026  
**Versión**: 1.0
