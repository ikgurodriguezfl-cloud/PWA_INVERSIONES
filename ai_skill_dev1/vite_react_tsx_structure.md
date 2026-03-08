my-enterprise-monorepo/          # Carpeta raíz del monorepo
├── .github/                     # Workflows de CI/CD para todos los proyectos
├── .husky/                      # Hooks de Git compartidos
├── .vscode/                     # Configuración global de VSCode
├── packages/                    # Librerías compartidas (design system, utils, etc.)
│   ├── ui-library/              # Librería interna de componentes UI
│   │   ├── src/
│   │   ├── package.json
│   │   └── tsconfig.json
│   ├── utils/                   # Funciones utilitarias compartidas
│   │   ├── src/
│   │   ├── package.json
│   │   └── tsconfig.json
│   └── types/                   # Tipos globales compartidos
│       ├── src/
│       ├── package.json
│       └── tsconfig.json
├── projects/                    # Múltiples aplicaciones/proyectos
│   ├── project-a/               # Proyecto A (ej. dashboard interno)
│   │   ├── public/
│   │   ├── src/                 # Aquí se define la estructura completa
│   │   │   ├── assets/          # Recursos estáticos (imágenes, fuentes, estilos globales)
│   │   │   ├── components/      # Componentes reutilizables
│   │   │   │   └── ui/          # Atomic design: atoms, molecules, organisms
│   │   │   ├── features/        # Módulos funcionales
│   │   │   │   └── auth/        # Ejemplo: autenticación
│   │   │   │       ├── api/     # Llamadas a servicios relacionados
│   │   │   │       ├── components/
│   │   │   │       ├── hooks/
│   │   │   │       ├── types.ts
│   │   │   │       └── index.ts
│   │   │   ├── hooks/           # Hooks globales
│   │   │   ├── layouts/         # Layouts generales
│   │   │   ├── pages/           # Páginas principales
│   │   │   ├── routes/          # Configuración de rutas
│   │   │   ├── services/        # Servicios externos
│   │   │   ├── store/           # Estado global
│   │   │   ├── styles/          # Estilos globales
│   │   │   ├── utils/           # Funciones utilitarias
│   │   │   ├── types/           # Tipos globales
│   │   │   ├── App.tsx          # Componente raíz
│   │   │   ├── main.tsx         # Punto de entrada
│   │   │   └── vite-env.d.ts    # Tipos generados por Vite
│   │   ├── tests/               # Pruebas unitarias e integración
│   │   │   └── e2e/             # Pruebas end-to-end
│   │   ├── index.html
│   │   ├── package.json
│   │   ├── tsconfig.json
│   │   └── vite.config.ts
│   ├── project-b/               # Proyecto B (ej. landing page)
│   │   ├── public/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── index.html
│   │   ├── package.json
│   │   ├── tsconfig.json
│   │   └── vite.config.ts
│   └── project-c/               # Proyecto C (ej. portal de clientes)
│       ├── public/
│       ├── src/
│       ├── tests/
│       ├── index.html
│       ├── package.json
│       ├── tsconfig.json
│       └── vite.config.ts
├── node_modules/                # Dependencias instaladas
├── package.json                 # Configuración raíz (workspaces)
├── pnpm-workspace.yaml          # Configuración de workspaces (pnpm)
├── tsconfig.base.json           # Configuración base de TypeScript compartida
└── README.md                    # Documentación general del monorepo

