# 🧪 Sakura Testing Skill

**Versión**: 1.0  
**Fecha Creación**: 12 de Marzo 2026  
**Asignado a**: `fic_sakura_agent_tester1`  
**Status**: ✅ Operativo  
**Categoría**: QA & Testing

---

## 📋 Descripción

Skill especializada en **QA testing exhaustivo**, **validación de cálculos financieros** y **detección de bugs críticos**. Garantiza que la solución funciona correctamente y los indicadores/señales son precisos.

---

## 🎯 Capacidades Principales

### 1. **Generación de Casos de Prueba (Test Case Generator)**
- Diseño de unit tests exhaustivos
- Casos de integración entre módulos
- Edge cases y boundary conditions
- Casos de error y validación
- Fixtures de datos realistas
- Casos de regresión preventiva

### 2. **Detección de Bugs (Bug Detector)**
- Smoke testing de funcionalidad principal
- Regression testing tras cambios
- Edge case verification
- Boundary testing (valores extremos)
- Detección de falsos positivos en señales
- Validación de comportamiento inesperado

### 3. **Validación de Calidad (Quality Validator)**
- Análisis de code coverage (target: >80%)
- Benchmarking de rendimiento
- Cumplimiento de estándares
- Validación de best practices
- Precisión de indicadores vs referencias (TradingView)
- Completitud de funcionalidades

### 4. **Testing de Regresión (Regression Tester)**
- Configuración de suite de regresión automatizada
- Testing automático tras cambios
- Análisis de impacto de cambios
- Comparativa antes/después
- Garantía de integridad histórica
- Validación de reproducibilidad

### 5. **Testing Financiero Específico**
- Validación de cálculos de indicadores técnicos
- Testing de estrategias de trading
- Rebalancing de portafolio
- Cálculos de riesgo y P&L
- Casos de opciones y derivados

### 6. **Testing de Integración**
- Integración con APIs de brokers
- Flujos end-to-end de trading
- Sincronización de datos
- Handling de errores de conexión
- Recuperación de fallos

### 7. **Testing de Seguridad**
- Validación de inputs maliciosos
- Protección contra inyecciones
- Encriptación de datos sensibles
- Testing de autenticación
- Control de acceso

### 8. **Performance Testing**
- Stress testing bajo carga alta
- Load testing de feeds de mercado
- Testing de escalabilidad
- Memory leaks detection
- Latency validation

---

## 📥 Entradas Típicas

- Código implementado y optimizado (de Naruto + Sasuke)
- Especificación de requisitos funcionales
- Datos de mercado de prueba
- Indicadores de referencia
- Criterios de aceptación

---

## 📤 Salidas Típicas

- Suite de tests automatizados (.test.ts)
- Reporte de bugs encontrados
- Métricas de code coverage
- Validación de precisión de indicadores
- Reporte de calidad final
- Documentación de casos de prueba

---

## 🔄 Integración en Fases

### FASE 3: Unit Testing
- Generar tests para cada módulo
- Validar funciones individuales
- Testing de edge cases

### FASE 3: Integration Testing
- Testing de flujos completos
- Integración con brokers
- Testing de APIs internas

### FASE 3: Quality Gate
- Validar code coverage >80%
- Verificar precisión de indicadores
- Confirmar latencia <100ms
- Aprobar para producción

---

## 💡 Consideraciones Especiales (Trading/Inversiones)

### Precisión Crítica
- **Indicadores Técnicos**: Validar vs TradingView (máximo 1% diferencia)
- **Cálculos Financieros**: Exactitud en decimales (no truncar)
- **Señales**: Validar reproducibilidad con datos históricos
- **Estrategias**: Backtesting con datos reales

### Casos de Prueba Críticos
- RSI, MACD, Bandas Bollinger con valores estándar
- Estrategia de opciones con casos extremos
- SMA/EMA con períodos dinámicos
- Manejo de mercados en gap (datos faltantes)
- Cambio de divisas y tipos de cambio

### Validación de Comportamiento
- Señales BUY/SELL correctas basadas en condiciones
- Activación/desactivación de alerts
- Manejo correcto de dividendos y splits
- Recuperación de desconexiones

### Performance Mínimos
- Unit tests ejecutan en <5ms
- Integration tests en <500ms
- Full suite en <30 segundos
- Coverage mínimo 80%

### Bugs Críticos a Detectar
- Cálculos de indicadores incorrectos
- Falsos positivos en señales
- Memory leaks en procesamiento de datos
- Pérdida de sincronización con broker
- Exposición de datos sensibles en logs

---

## 🛠️ Herramientas y Librerías

### Testing Framework
- Jest para unit tests
- Vitest como alternativa (más rápido)
- Supertest para APIs
- Cypress para E2E (si hay UI)

### Financial Testing
- TA-Lib para validar indicadores
- Manual calculation scripts
- TradingView API para comparación (si aplica)

### Data & Fixtures
- Faker.js para datos sintéticos
- Histórico real de mercados
- Casos extremos documentados

### Monitoring & Reporting
- Coverage reports (Istanbul/NYC)
- Allure reports
- GitHub Actions para CI/CD
- Slack notifications para fails críticos

---

## 📊 Matriz de Pruebas Recomendada

| Componente | Unit | Integration | Performance | Security |
|-----------|------|-------------|-------------|----------|
| Indicadores TA | ✅ | ✅ | ✅ | - |
| Motor de Señales | ✅ | ✅ | ✅ | ✅ |
| API Broker | - | ✅ | ✅ | ✅ |
| Portfolio Manager | ✅ | ✅ | ✅ | - |
| Autenticación | ✅ | ✅ | ✅ | ✅ |

