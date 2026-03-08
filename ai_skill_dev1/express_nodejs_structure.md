my-enterprise-api-monorepo/       # Carpeta raíz del monorepo
├── .github/                      # Workflows de CI/CD para todos los proyectos
├── .husky/                       # Hooks de Git compartidos
├── .vscode/                      # Configuración global de VSCode
├── packages/                     # Librerías compartidas (middlewares, utils, etc.)
│   ├── middleware/               # Middlewares comunes (auth, logging, error handling)
│   │   ├── src/
│   │   ├── package.json
│   │   └── tsconfig.json
│   ├── utils/                    # Funciones utilitarias compartidas
│   │   ├── src/
│   │   ├── package.json
│   │   └── tsconfig.json
│   └── types/                    # Tipos globales compartidos
│       ├── src/
│       ├── package.json
│       └── tsconfig.json
├── projects/                     # Múltiples APIs/proyectos
│   ├── project-a/                # Proyecto A (ej. API de usuarios)
│   │   ├── src/
│   │   │   ├── config/           # Configuración (env, db, server)
│   │   │   ├── controllers/      # Controladores (lógica de negocio)
│   │   │   ├── routes/           # Definición de rutas RESTful
│   │   │   ├── models/           # Modelos (ORM/ODM: Sequelize, Mongoose)
│   │   │   ├── services/         # Servicios externos (APIs, colas, etc.)
│   │   │   ├── middlewares/      # Middlewares específicos del proyecto
│   │   │   ├── utils/            # Funciones utilitarias locales
│   │   │   ├── tests/            # Pruebas unitarias e integración
│   │   │   ├── app.ts            # Configuración de Express
│   │   │   └── server.ts         # Punto de entrada del servidor
│   │   ├── package.json
│   │   ├── tsconfig.json
│   │   └── README.md
│   ├── project-b/                # Proyecto B (ej. API de productos)
│   │   ├── src/
│   │   │   ├── config/
│   │   │   ├── controllers/
│   │   │   ├── routes/
│   │   │   ├── models/
│   │   │   ├── services/
│   │   │   ├── middlewares/
│   │   │   ├── utils/
│   │   │   ├── tests/
│   │   │   ├── app.ts
│   │   │   └── server.ts
│   │   ├── package.json
│   │   ├── tsconfig.json
│   │   └── README.md
│   └── project-c/                # Proyecto C (ej. API de órdenes)
│       ├── src/
│       │   ├── config/
│       │   ├── controllers/
│       │   ├── routes/
│       │   ├── models/
│       │   ├── services/
│       │   ├── middlewares/
│       │   ├── utils/
│       │   ├── tests/
│       │   ├── app.ts
│       │   └── server.ts
│       ├── package.json
│       ├── tsconfig.json
│       └── README.md
├── node_modules/                 # Dependencias instaladas
├── package.json                  # Configuración raíz (workspaces)
├── pnpm-workspace.yaml           # Configuración de workspaces (pnpm)
├── tsconfig.base.json            # Configuración base de TypeScript compartida
└── README.md                     # Documentación general del monorepo

