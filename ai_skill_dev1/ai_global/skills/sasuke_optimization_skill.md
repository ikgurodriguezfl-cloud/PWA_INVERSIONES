# ⚡ Sasuke Optimization Skill

**Versión**: 1.0  
**Fecha Creación**: 12 de Marzo 2026  
**Asignado a**: `fic_sasuke_agent_dev2`  
**Status**: ✅ Operativo  
**Categoría**: Optimización & Seguridad

---

## 📋 Descripción

Skill especializada en **optimización de rendimiento**, **auditoría de seguridad** y **refactoring de código**. Garantiza que la implementación de Naruto cumpla requisitos de latencia, seguridad y best practices.

---

## 🎯 Capacidades Principales

### 1. **Optimización de Rendimiento (Code Optimizer)**
- Identificar y eliminar cuellos de botella
- Optimizar loops y búsquedas O(n²) → O(n log n)
- Memory profiling y reducción de footprint
- Lazy loading y code splitting
- Caching strategies (LRU, TTL)
- Batch processing de actualizaciones

### 2. **Análisis de Rendimiento (Performance Analyzer)**
- Profiling de ejecución (CPU, memory)
- Detección de memory leaks
- Bottleneck analysis detallado
- Stress testing bajo carga realista
- Benchmarking comparativo (antes/después)
- Monitoring de métricas en tiempo real

### 3. **Auditoría de Seguridad (Security Auditor)**
- Static security analysis (SAST)
- Detección de secrets en código (API keys, tokens)
- Análisis de dependencias vulnerables
- Review de variables de entorno
- Validación de inputs y sanitización
- Encriptación de datos sensibles
- Control de acceso y permisos

### 4. **Refactoring de Código (Pattern Refactorer)**
- Aplicación de principios SOLID
- Consolidación de código duplicado (DRY)
- Implementación de design patterns
- Mejora de reusabilidad de componentes
- Simplificación de lógica compleja
- Mejora de legibilidad y mantenibilidad

### 5. **Mejora de Arquitectura**
- Desacoplamiento de módulos
- Abstracción de dependencias
- Composición sobre herencia
- Inyección de dependencias

### 6. **Testing Performance**
- Generación de casos de rendimiento
- Automación de benchmarks
- Validación de SLAs de latencia
- Comparativa antes/después optimizaciones

### 7. **Documentación de Optimizaciones**
- Registro de cambios realizados
- Justificación de decisiones
- Benchmarks documentados
- Recomendaciones para futuro

### 8. **Code Quality Tools**
- ESLint, Prettier enforcement
- TypeScript strict mode validation
- Dependency audits
- Bundle size analysis

---

## 📥 Entradas Típicas

- Código implementado por Naruto
- Especificación de requisitos de rendimiento
- Reporte de bugs o problemas de latencia
- Código legacy a refactorizar
- Análisis de seguridad requerido

---

## 📤 Salidas Típicas

- Código optimizado y refactorizado
- Reporte de rendimiento con benchmarks
- Reporte de seguridad y vulnerabilidades
- Documentación de cambios
- Recomendaciones para mejora continua

---

## 🔄 Integración en Fases

### FASE 3: Optimización
- Revisar código de Naruto
- Ejecutar profiling y analysis
- Identificar cuellos de botella críticos
- Implementar optimizaciones

### FASE 3: Seguridad
- Auditar dependencias y secretos
- Validar manejo de datos sensibles
- Verificar variables de entorno
- Documentar issues y fixes

### FASE 3: Refactoring
- Consolidar código duplicado
- Mejorar patrones de diseño
- Aumentar reusabilidad
- Documentar decisiones

---

## 💡 Consideraciones Especiales (Trading/Inversiones)

### Requisitos Críticos
- **Latencia**: <100ms en actualización de señales de mercado
- **Precision**: Exactitud en cálculos financieros (no perder decimales)
- **Memory**: Gestión eficiente de datos históricos grandes
- **Seguridad**: API keys y tokens NUNCA expuestos

### Patrones Críticos a Optimizar
- Procesamiento de feeds de WebSocket (evitar lag)
- Cálculo de indicadores (TA) en datasets grandes
- Updates de estado de posiciones (frecuentes)
- Queries a base de datos histórica

### Benchmarks Esperados
- Actualización de indicadores: <50ms
- Generación de señales: <100ms
- Update de UI con nuevos datos: <16ms (60fps)
- API calls a broker: <200ms

### Seguridad Crítica
- **API Keys**: NO hardcodeadas, variables de entorno
- **Tokens**: Refresh tokens y expiración
- **Data**: Encripción en tránsito, validación de inputs
- **Logs**: NO registrar datos sensibles

---

## 🛠️ Herramientas y Librerías

### Profiling & Monitoring
- Node.js Profiler / Chrome DevTools
- New Relic, Datadog (opcional)
- Jest performance benchmarks
- Lighthouse (para frontend)

### Security
- npm audit, Snyk, OWASP
- dotenv-safe para variables
- crypto-js para encriptación basic

### Code Quality
- ESLint, Prettier
- SonarQube (opcional)
- Dependency Check tools
