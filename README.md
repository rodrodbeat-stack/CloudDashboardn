# NEURA SOCIAL v3 — Neural Audio 2050

Frontend responsive con estética cyberpunk/industrial, álbumes, comunidad demo, feed de reels, reproductor, perfil editable y formulario de publicación.

## Ejecutar
Abre `index.html` o publica la carpeta en GitHub Pages. Para pruebas locales puedes usar VS Code Live Server.

## Estado funcional
- Navegación por secciones, reproductor de interfaz, tarjetas de álbum y feed.
- Publicaciones y perfil se guardan en `localStorage` del navegador.
- El formulario permite adjuntar imagen, audio o vídeo y muestra el nombre del archivo en el post. El archivo no se sube a un servidor en esta versión.
- La autenticación, sincronización multiusuario y almacenamiento remoto requieren conectar un proyecto Supabase.

## Activar backend real
1. Crea un proyecto Supabase.
2. Ejecuta `supabase-schema.sql` en SQL Editor.
3. Crea un bucket `neura-media` en Storage y define políticas de acceso autenticado.
4. Integra la URL del proyecto y la clave publicable en un archivo de configuración frontend. Nunca incluyas `service_role` en el navegador.

Esta entrega no incluye credenciales ni afirma que el backend esté conectado.
