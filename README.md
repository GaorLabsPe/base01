# Base de Tienda Online v2 - E-commerce Genérico

Esta es una plantilla de e-commerce moderna, adaptable y de alto rendimiento, diseñada para ser personalizada y desplegada rápidamente. La versión 2 introduce un archivo de configuración centralizado para facilitar la personalización.

## Características Principales

- **Adaptable (Responsive):** Funciona en cualquier dispositivo, desde móviles hasta ordenadores de escritorio.
- **Modo Oscuro y Claro:** Interfaz personalizable para la preferencia del usuario.
- **Panel de Administración Integrado:** Gestiona productos, pedidos y clientes sin salir de la tienda.
- **Configuración Sencilla:** Personaliza tu tienda editando un único archivo `config.js`.
- **Despliegue Rápido:** Lista para desplegar en plataformas como Vercel, Netlify o Firebase Hosting.

## Vista Previa

*Próximamente se añadirá una vista previa en vivo.*

## Cómo Empezar

Sigue estos pasos para configurar y lanzar tu tienda:

### 1. Clona el Repositorio

```bash
git clone https://github.com/GaorLabsPe/base01.git
cd base01
```

### 2. Configura tu Tienda

Todos los ajustes importantes se encuentran en el archivo `config.js`. Ábrelo y modifica los siguientes campos:

- **`supabase`**: Reemplaza `YOUR_SUPABASE_URL` y `YOUR_SUPABASE_ANON_KEY` con las credenciales de tu proyecto de Supabase. Las encontrarás en **Settings > API** en tu panel de Supabase.
- **`businessName`**: El nombre de tu negocio.
- **`businessSubtitle`**, **`slogan`**, **`description`**: Textos para personalizar la identidad de tu tienda.
- **`contact`** y **`social`**: Información de contacto y enlaces a redes sociales.

### 3. Ejecuta el Proyecto

Para desarrollar y probar en tu máquina local, necesitas tener [Node.js](https://nodejs.org/) instalado. Luego, ejecuta:

```bash
npm install
npm run dev
```

Esto iniciará un servidor de desarrollo local, y podrás ver tu tienda en `http://localhost:5173`.

### 4. Configura la Base de Datos

Para que la tienda funcione, necesitas crear las tablas en tu base de datos Supabase:

1.  Ve a tu proyecto de Supabase.
2.  En el menú de la izquierda, selecciona **SQL Editor**.
3.  Haz clic en **New query**.
4.  Copia y pega el script SQL que encontrarás en la sección de **Configuración > Paso 1** del panel de administración de tu tienda.
5.  Haz clic en **RUN**.

### 5. Crea Usuarios Administradores

Por seguridad, los usuarios administradores se crean desde el panel de Supabase:

1.  Ve a **Authentication > Users** en tu panel de Supabase.
2.  Crea un nuevo usuario (o varios) que utilizarás para gestionar la tienda.

### 6. Despliega tu Tienda

Una vez que tu tienda esté configurada, puedes desplegarla en cualquier servicio de hosting estático como Vercel, Netlify o Firebase Hosting.

## Tecnologías Utilizadas

- HTML5, CSS3, JavaScript (ES6+)
- [Supabase](https://supabase.io) como backend (Base de datos, Autenticación).
- [Cloudinary](https://cloudinary.com) para la gestión de imágenes de productos.
- [Vite](https://vitejs.dev) para un entorno de desarrollo rápido.
- [Chart.js](https://www.chartjs.org) para los gráficos del dashboard.

## Contribuciones

Las contribuciones son bienvenidas. Si tienes ideas para mejorar la plantilla, no dudes en abrir un *issue* o enviar un *pull request*.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
