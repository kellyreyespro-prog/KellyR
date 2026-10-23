# Mi Ritual · v0.1

Versión inicial publicable del sitio de autocuidado.

## Autenticación

Se requiere configurar **Supabase Auth** y la tabla `ritual_profiles` con políticas RLS antes de abrir el sitio a usuarios. No existe acceso de invitado ni se incluyen contraseñas. En `index.html` configure `window.RITUAL_CLOUD` usando solo la URL del proyecto y la clave pública (publishable), **nunca** `service_role` ni secretos.

Los formularios de perfil recogen información sensible. Antes de producción, verificar privacidad, RLS, consentimiento y borrado de datos.
