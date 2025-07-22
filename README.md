# 🔐 Autenticación de Usuarios – React + Node.js + MongoDB

Este proyecto es una aplicación **full stack** que implementa un sistema de autenticación de usuarios usando:

- **Frontend:** React + Fetch API + React Router DOM  
- **Backend:** Node.js + Express + MongoDB + JWT + bcrypt

Está diseñado como un ejemplo real de cómo funcionan los flujos de registro e inicio de sesión en aplicaciones modernas, incluyendo manejo de **tokens JWT**, validaciones, y protección de rutas.

<br>



## 🚀 Funcionalidades principales

- ✔️ Registro de nuevos usuarios con validación de datos  
- ✔️ Inicio de sesión seguro con verificación de credenciales  
- ✔️ Contraseñas cifradas con **bcrypt**  
- ✔️ Generación y almacenamiento de **tokens JWT** en el navegador  
- ✔️ Backend con rutas protegidas usando middleware  
- ✔️ Feedback en tiempo real desde el backend al frontend  
- ✔️ Conexión a base de datos **MongoDB** con Mongoose  

<br>



## 🛠️ Tecnologías utilizadas

### 🔧 Backend
- **Node.js** + **Express**
- **MongoDB** + **Mongoose**
- **bcryptjs** para hashear contraseñas
- **jsonwebtoken** para generar tokens JWT
- **dotenv** para variables de entorno
- **CORS** para permitir conexiones con el frontend

### 🎨 Frontend
- **React** (funcional, con hooks)
- **React Router DOM** para la navegación
- **Fetch API** para conectar con el backend
- **LocalStorage** para guardar el token JWT

<br>



## 🧩 Estructura del proyecto
```
mi-proyecto-auth/
│ 
├── back - nodejs/
│ ├── middlewares/
│ │ └── authMiddleware.js
│ ├── models/
│ │ └── Usuario.js
│ ├── routes/
│ │ └── authRoutes.js
│ ├── .env
│ ├── server.js
│ └── node_modules/
│   └── package-lock.json
│   └── package.json
│ 
├── front - react/
│ ├── .vite
│ ├── node_modules/
│ ├── src/
│   └──pages/
│   │ ├── Login.jsx
│   │ └── Register.jsx
│   └── App.jsx
│   └── Main.jsx
│   └── styles.css
│ 
└── .gitignore
```

<br>



## ⚙️ Configurar el backend

1. Entrá a la carpeta del backend:
   
```bash
cd back - nodejs
```

2. Instala todas las dependencias necesarias:

```bash
npm install express mongoose bcryptjs jsonwebtoken cors dotenv
```
  
3. Creá un archivo .env dentro de la carpeta components y agregá tu clave secreta para los tokens:

```bash
JWT_SECRET=mitokensecreto123
```
   
4. Asegurarse que MongoDB este corriendo localmente, la URL utilizada es:

```bash
mongodb://localhost:27017/nombre-random
```

<br>


## ⚙️ Configurar el frontend


1. Entrá a la carpeta del frontend:
   
```bash
cd front - react
```

2. Instala todas las dependencias necesarias:

```bash
npm install react react-dom react-router-dom
```
  
3. Ejecutar el proyecto:

```bash
npm run dev
```
   
