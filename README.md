# Ga$tify Frontend

## 📱 Aplicación Móvil de Gestión de Gastos Personales

Ga$tify es una aplicación móvil diseñada para transformar la manera en que las personas gestionan sus finanzas personales, ofreciendo una plataforma accesible, automatizada y educativa con análisis inteligentes y visualización clara de gastos.

## 🚀 Guía de Instalación y Ejecución

### Prerrequisitos

Antes de comenzar, asegúrate de tener instalado:

- **Node.js** (versión 18.x o superior)
- **npm** (viene con Node.js)
- **Git**

### Verificar instalaciones

```bash
# Verificar Node.js
node --version

# Verificar npm
npm --version

# Verificar Git
git --version
```

### 1. Clonar el repositorio

```bash
# Clonar el repositorio frontend
git clone https://github.com/GermanMorenoBauer/gastify-frontend.git

# Entrar al directorio del proyecto
cd gastify-frontend
```

### 2. Instalar dependencias

```bash
# Instalar todas las dependencias del proyecto
npm install
```

### 3. Ejecutar el proyecto

```bash
# Iniciar el servidor de desarrollo
npm start

# O alternativamente
ng serve
```

### 4. Acceder a la aplicación

Una vez que el servidor esté corriendo, abre tu navegador y ve a:

```
http://localhost:4200
```

## 📋 Comandos Útiles

```bash
# Instalar dependencias
npm install

# Ejecutar en modo desarrollo
npm start
ng serve

# Ejecutar en modo desarrollo con recarga automática
ng serve --watch

# Construir para producción
npm run build
ng build

# Ejecutar tests
npm test
ng test

# Ejecutar linting
npm run lint
ng lint

# Verificar el estado del proyecto
ng version
```

## 🏗️ Estructura del Proyecto

```
gastify-frontend/
├── src/
│   ├── app/
│   │   ├── pages/
│   │   │   ├── welcome/          # Pantalla de bienvenida
│   │   │   ├── login/            # Pantalla de login
│   │   │   └── register/         # Pantalla de registro
│   │   ├── app.component.html    # Componente principal
│   │   ├── app.component.ts
│   │   ├── app.component.scss
│   │   ├── app.routes.ts         # Configuración de rutas
│   │   └── app.config.ts
│   ├── assets/
│   │   └── images/
│   │       ├── gastifyLogo.png   # Logo principal
│   │       └── google-icon.png   # Icono de Google
│   ├── styles.scss               # Estilos globales
│   └── index.html
├── package.json
├── angular.json
├── tsconfig.json
└── README.md
```

## 🎨 Tecnologías Implementadas

### Frontend
- **Angular 18** - Framework principal
- **TypeScript** - Lenguaje de programación
- **SCSS** - Preprocesador de CSS
- **Material Design Icons (MDI)** - Biblioteca de iconos
- **Responsive Design** - Diseño adaptable

### Características Implementadas
- ✅ **Pantalla de Bienvenida** - Landing page con logo y botones de acción
- ✅ **Pantalla de Login** - Formulario de autenticación con Google
- ✅ **Pantalla de Registro** - Formulario de registro de usuarios
- ✅ **Diseño Responsive** - Adaptable a móviles, tablets y desktop
- ✅ **Paleta de Colores Ga$tify** - Colores personalizados de la marca

## 🎨 Paleta de Colores

```scss
// Colores principales de Ga$tify
--gastify-dark: #0F152C;      // Fondo principal
--gastify-green: #3DCD99;     // Verde principal
--gastify-purple: #3B3B58;    // Púrpura secundario
--gastify-blue: #15233C;      // Azul oscuro
--gastify-light: #FFFFFF;     // Blanco/azul claro
```

## 📱 Pantallas Implementadas

### 1. Pantalla de Bienvenida (`/`)
- Logo de Ga$tify prominente
- Título y subtítulo descriptivos
- Botones de acción: "Crear cuenta" e "Iniciar sesión"
- Características destacadas con iconos MDI
- Diseño completamente responsive

### 2. Pantalla de Login (`/login`)
- Logo de Ga$tify
- Formulario de login con campos de email/username y contraseña
- Botón de "Conectar con Google"
- Enlaces de "¿Olvidaste tu contraseña?" y "Registrate"
- Diseño responsive y accesible

### 3. Pantalla de Registro (`/register`)
- Logo de Ga$tify
- Formulario completo de registro
- Campos: username, email, contraseña, confirmar contraseña, fecha de nacimiento
- Checkbox de términos y condiciones
- Botón "Siguiente" para continuar
- Diseño responsive

## 🔧 Configuración del Entorno

### Variables de Entorno
El proyecto está configurado para trabajar con variables de entorno. Crea un archivo `.env` en la raíz del proyecto si necesitas configuraciones específicas.

### Configuración de Angular
- **TypeScript**: Configurado para Angular 18
- **SCSS**: Preprocesador de estilos
- **Routing**: Configurado con rutas standalone
- **Assets**: Configurados para imágenes y recursos

## 🚀 Desarrollo

### Estructura de Componentes
Todos los componentes están configurados como **standalone components** siguiendo las mejores prácticas de Angular 18.

### Estilos
- **SCSS** para estilos modulares
- **Variables CSS** para la paleta de colores
- **Media queries** para diseño responsive
- **Fuente Poppins** importada desde Google Fonts

### Iconos
- **Material Design Icons (MDI)** para iconografía consistente
- Iconos personalizados para funcionalidades específicas

## 🔗 Integración con Backend

El frontend está preparado para integrarse con el backend de Ga$tify:

- **APIs REST** para autenticación y gestión de datos
- **JWT** para manejo de sesiones
- **MongoDB** como base de datos
- **Node.js + TypeScript** en el backend

## 📱 Responsive Design

La aplicación está optimizada para:
- 📱 **Móviles** (320px - 480px)
- 📱 **Tablets** (481px - 768px)
- 💻 **Desktop** (769px+)

## 🐛 Solución de Problemas

### Error: "Could not find the '@angular-devkit/build-angular:dev-server'"
```bash
npm install
npm start
```

### Error: "Node packages may not be installed"
```bash
rm -rf node_modules package-lock.json
npm install
```

### Error: "Port 4200 is already in use"
```bash
# Usar un puerto diferente
ng serve --port 4201
```

### Error: "Module not found"
```bash
npm install
npm start
```

## 📝 Scripts Disponibles

```bash
# Desarrollo
npm start          # Inicia el servidor de desarrollo
npm run build      # Construye para producción
npm run test       # Ejecuta tests
npm run lint       # Ejecuta linting

# Angular CLI
ng serve           # Servidor de desarrollo
ng build           # Construcción
ng test            # Tests
ng lint            # Linting
```

## 🤝 Contribución

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 👥 Equipo

- **Germán Moreno Bauer** - Desarrollador Full Stack
- **Contacto**: [Tu email de contacto]

## 🚀 Roadmap

### Próximas Funcionalidades
- [ ] Dashboard principal con gráficos
- [ ] Registro de gastos manual
- [ ] Integración con WhatsApp Bot
- [ ] Análisis inteligente con OpenAI
- [ ] Configuración de perfil de usuario
- [ ] Notificaciones push
- [ ] Exportación de reportes

### Mejoras Técnicas
- [ ] Implementación de PWA
- [ ] Optimización de performance
- [ ] Tests unitarios y de integración
- [ ] CI/CD pipeline
- [ ] Deploy automático

---

**¡Gracias por usar Ga$tify! 💚**
