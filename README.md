# Backend - Workspace

Este proyecto es una API RESTful construida con Node.js, Express y MongoDB que permite la gestion de espacios de trabajo (Workspaces) con autenticacion segura.

# Tecnologias utilizadas
- **Node.js & Express**: Servidor web
- **MongoDB & Mongoose**: Base de datos
- **JWT (JsonWebToken)**: Autenticacion
- **Nodemailer**: Envio de correos de verificacion e invitacion.

# Instalacion

1. Clonar el repositorio.
2. Instalar dependencias:
    npm install
3. Configurar las variables de entorno:
    Renombrar el archivo .env.example a .env.
    Completar los datos de conexion.
4. Iniciar el servidor:
    npm run dev

# Endpoints Principales

# Auth
    POST /api/auth/register: Registrar usuario.

    POST /api/auth/login: Iniciar sesion.

# Workspace (Requiere Token)
    GET /api/workspace: Listar mis espacios.

    POST /api/workspace: Crear espacio.

    PATCH /api/workspace/:id: Editar espacio.

    DELETE /api/workspace/:id: Eliminar espacio.