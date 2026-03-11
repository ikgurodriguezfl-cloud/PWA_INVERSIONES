# 🎨 Frontend Design Skill

**Versión**: 1.0  
**Fecha Creación**: 11 de Marzo 2026  
**Asignado a**: `fic_naruto_agent_dev1`  
**Status**: ✅ Operativo  
**Categoría**: Diseño & Implementación Visual

---

## 📋 Descripción

Skill especializada en **diseño de interfaces frontend** y **arquitectura visual** de componentes React. Cubre desde diseño atómico hasta layouts complejos, respuesta, accesibilidad y experiencia de usuario.

---

## 🎯 Capacidades Principales

### 1. **Atomic Design Architecture**
- Crear sistema de componentes atoms, molecules, organisms
- Definir propiedades y variantes
- Composición de componentes complejos
- Documentación de componentes

### 2. **Design System Implementation**
- Paleta de colores y tokens de diseño
- Tipografía y escalas
- Espaciado y grillas
- Componentes reutilizables consistentes

### 3. **Responsive Design**
- Mobile-first approach
- Media queries y breakpoints
- Fluid typography y spacing
- Tests responsivos

### 4. **Accesibilidad (A11y)**
- WCAG 2.1 compliance
- ARIA labels y roles
- Keyboard navigation
- Contraste y legibilidad

### 5. **UI Patterns & Best Practices**
- Form design y validation visual
- Loading states y error handling
- Unidirectional data flow visual
- State management patterns (Zustand)

### 6. **Interactive Components**
- Transiciones y animaciones suaves
- Micro-interactions
- Feedback visual inmediato
- Performance de animaciones

### 7. **Trading/Finance UI Specific**
- Layouts para dashboards financieros
- Visualización de datos de mercado
- Tablas de datos complejas
- Indicadores visuales de estado

### 8. **Tailwind CSS Mastery**
- Utility-first approach
- Custom configurations
- Responsive classes
- Plugin development si es necesario

---

## 📥 Entradas Típicas

- Especificación de requisitos UI/UX
- Wireframes o mockups de diseñador
- Design tokens y brand guidelines
- Datos a visualizar (market data, signals, portfolio)

---

## 📤 Salidas Típicas

- Componentes React reutilizables (.tsx)
- Estilos Tailwind optimizados
- Design tokens configurados
- Documentación de componentes
- Ejemplos de uso (Storybook-ready)

---

## 🔄 Integración en Fases

### FASE 2.4: Estructura Base
- Definir design tokens
- Crear archivo de configuración Tailwind
- Estructura carpetas de componentes
- Base styles y reset

### FASE 3: Implementación
- Implementar atomic components
- Layouts principales
- Componentes específicos de trading
- Animaciones y transiciones

---

## 📐 Estándares de Implementación

### Naming Convention
```
atoms/         → Button, Input, Badge, Card
molecules/     → FormField, NavBar, SignalCard
organisms/     → Dashboard, Watchlist, Portfolio
```

### Estructura de Componente
```tsx
// FIC: Component type definition and documentation (EN)
// FIC: Definición de tipo de componente y documentación (ES)
interface ComponentProps {
  variant?: 'primary' | 'secondary';
  size?: 'sm' | 'md' | 'lg';
  disabled?: boolean;
  children: React.ReactNode;
}

// FIC: Exported component with proper typing (EN)
// FIC: Componente exportado con tipado correcto (ES)
export const Component: React.FC<ComponentProps> = ({
  variant = 'primary',
  size = 'md',
  disabled = false,
  children,
}) => {
  return (
    <div className={`component component--${variant} component--${size}`}>
      {children}
    </div>
  );
};
```

### Tailwind Best Practices
- Usar clases del framework, evitar CSS custom innecesario
- Responsive prefixes: `sm:`, `md:`, `lg:`, `xl:`, `2xl:`
- Dark mode support cuando aplique
- Accesibilidad: `focus:`, `hover:`, `disabled:`, `aria-*`

---

## 🧪 Criterios de Aceptación

### Componentes
- [ ] Props TypeScript completamente tipados
- [ ] Accesibilidad WCAG cumplida
- [ ] Responsivo en mobile, tablet, desktop
- [ ] Comentarios FIC en secciones complejas
- [ ] Ejemplos de uso documentados
- [ ] Sin hardcoding de colores (usar tokens)

### Layouts
- [ ] Grid/Flex correctamente utilizado
- [ ] Responden a distintos tamaños de pantalla
- [ ] Contenido reflow sin quiebre
- [ ] Performance: no layout thrashing

### Animaciones
- [ ] 60fps si es posible
- [ ] Transiciones suaves
- [ ] Respetan `prefers-reduced-motion`
- [ ] Performance optimizado

---

## 🚀 Skills Complementarias

- `react_code_generator` - Integración de componentes en features
- `typescript_code_generator` - Tipado avanzado de componentes
- `code_optimizer` (Sasuke) - Optimización CSS y performance
- `documentation_writer` - Documentar componentes

---

## 📚 Recursos de Referencia

- [Atomic Design by Brad Frost](https://atomicdesign.bradfrost.com/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [WAI-ARIA Authoring Practices](https://www.w3.org/WAI/ARIA/apg/)
- [React Best Practices](https://react.dev)
- [Web Accessibility Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)

---

## 🔗 Relación con Otros Skills

```
[architecture_designer] (Kakashi)
    ↓ define estructura visual
[frontend_design] (Naruto) ← TÚ ERES AQUÍ
    ↓ entrega componentes
[react_code_generator] (Naruto)
    ↓ integra en features
[code_optimizer] (Sasuke)
    ↓ optimiza CSS/rendering
```

---

## ✅ Estado del Skill

- **Creado**: 11 de Marzo 2026
- **Versión**: 1.0
- **Agentes**: fic_naruto_agent_dev1
- **Fases**: 2.4, 3
- **Prioridad**: Alta
