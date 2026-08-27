# Blanca Nieves App v3 — sincronizada + ícono de aplicación

Esta versión corrige dos puntos:

1. **Sincronización real:** la aplicación ya no cae silenciosamente en almacenamiento local. Si Supabase no está conectado, muestra un error en vez de guardar datos distintos por dispositivo.
2. **Ícono PWA:** incluye `icon-192.png`, `icon-512.png` y `apple-touch-icon.png` generados a partir del logo de la Escuela de Lenguaje Blanca Nieves.

## Cómo actualizar el proyecto actual
En GitHub, repositorio `blanca-nieves-cuotas`, reemplaza/sube TODOS los archivos de este paquete en la raíz del repositorio y confirma los cambios en `main`.

Vercel detectará el commit y hará un despliegue nuevo automáticamente.

## Cómo comprobar la sincronización
1. Abre la app después del nuevo despliegue.
2. Debe aparecer la pantalla de inicio de sesión.
3. Inicia sesión con un usuario de Supabase Authentication.
4. Agrega un estudiante de prueba.
5. En Supabase > Table Editor > `students`, confirma que aparece.
6. Abre la app en otro dispositivo e inicia sesión: el mismo estudiante debe verse allí.

## Instalar con logo
Después del despliegue nuevo:
- Android/Chrome: menú ⋮ > **Instalar aplicación** o **Agregar a pantalla de inicio**.
- Computador/Chrome/Edge: botón de instalación en la barra de direcciones o menú > **Instalar Blanca Nieves**.

Si ya tenías una versión instalada, conviene desinstalarla y volver a instalarla para que tome el nuevo ícono.

Nunca uses ni publiques una clave `sb_secret_...` en el frontend.
