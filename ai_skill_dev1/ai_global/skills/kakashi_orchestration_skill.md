# 🧠 Kakashi Orchestration Skill

**Versión**: 1.0  
**Fecha Creación**: 12 de Marzo 2026  
**Asignado a**: `fic_kakashi_agent_orchestrator`  
**Status**: ✅ Operativo  
**Categoría**: Investigación & Arquitectura

---

## 📋 Descripción

Skill especializada en **investigación técnica**, **diseño arquitectónico** y **orquestación de soluciones** para plataformas de inversiones/trading. Convierte requisitos de negocio en arquitectura técnica robusta.

---

## 🎯 Capacidades Principales

### 1. **Análisis de Requisitos (Ticket Analysis)**
- Desglosar especificaciones en componentes técnicos
- Identificar dependencias entre requisitos
- Evaluar impacto de cambios
- Validar integridad y completitud de especificaciones
- Extraer criterios de aceptación técnicos

### 2. **Diseño Arquitectónico (Architecture Design)**
- Diseñar estructura de servicios y módulos
- Flujos de datos de mercado end-to-end
- Arquitectura de indicadores técnicos
- Motor de señales y estrategias
- Integración con brokers y APIs externas
- Patrones de escalabilidad

### 3. **Validación de Requisitos (Requirement Validation)**
- Detectar requisitos conflictivos
- Validar cobertura de casos de uso
- Verificar alineación con especificación
- Identificar gaps técnicos
- Evaluar factibilidad de implementación

### 4. **Síntesis de Conocimiento (Knowledge Synthesis)**
- Consolidar investigaciones de APIs de brokers
- Comparar librerías de indicadores técnicos
- Resumir estrategias de trading y opciones
- Implementar decisiones tecnológicas documentadas
- Generar base de conocimiento inicial del proyecto

### 5. **Decisiones Tecnológicas**
- Stack selection y justificación
- Elección de librerías especializadas
- Patrones arquitectónicos recomendados
- Trade-offs tecnológicos
- Mitigación de riesgos técnicos

### 6. **Documentación Arquitectónica**
- Diagramas de arquitectura
- Especificación de módulos y servicios
- Flujos de datos visuales
- Matriz de dependencias
- Decisiones registradas (ADR)

### 7. **Planificación de Fases**
- Descomposición en hitos
- Secuenciación de tareas
- Identificación de críticos
- Estimación de complejidad

### 8. **Investigación de Mercado & Tecnologías**
- Análisis de APIs de brokers (IB, Alpaca, etc.)
- Evaluación de librerías financieras (TA-Lib, Tulip)
- Estrategias de trading y risk management
- Best practices en trading algorítmico
- Regulaciones y compliance

---

## 📥 Entradas Típicas

- SPECIFICATION.md de proyecto
- Tickets externos o requisitos del cliente
- Reportes de investigación previa
- Decisiones de negocio o restricciones
- Métricas de rendimiento requeridas

---

## 📤 Salidas Típicas

- Arquitectura técnica definida
- Especificación de módulos (config.yaml)
- Knowledge base documentada
- Lista de requisitos técnicos validados
- Matriz de dependencias
- Decisiones arquitectónicas registradas
- Plan de implementación por fases

---

## 🔄 Integración en Fases

### FASE 2.3: Investigación
- Investigar APIs de brokers disponibles
- Analizar librerías de indicadores técnicos
- Documentar patrones de trading viables
- Validar requisitos vs especificación

### FASE 2.4: Diseño
- Diseñar arquitectura de módulos
- Especificar flujos de datos
- Definir interfaces de servicios
- Crear config.yaml con decisiones técnicas

### FASE 3: Soporte
- Validar implementación cumple arquitectura
- Coordinar con Naruto (implementación)
- Guiar decisiones de Sasuke (optimización)
- Revisar testing de Sakura

---

## 💡 Consideraciones Especiales (Trading/Inversiones)

### Requisitos Críticos
- **Latencia**: <100ms en actualizaciones de señales
- **Precisión**: Cálculos financieros exactos (decimales)
- **Integridad**: No perder datos de mercado
- **Seguridad**: API keys y datos sensibles protegidos

### Patrones Recomendados
- Event-driven para feeds de mercado
- Caching para datos históricos
- Queue systems para procesamiento de señales
- State management para posiciones y portafolios

### Integraciones Críticas
- Brokers API (WebSocket para tiempo real)
- Datos de mercado (precios, volúmenes)
- Librerías de cálculo financiero
- Bases de datos (histórico, posiciones)
