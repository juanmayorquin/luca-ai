---
title: Política de privacidad de Luca
---

# Política de privacidad de Luca

**Última actualización:** 2 de noviembre de 2026

## 1. Qué es Luca

Luca es un asistente personal de uso privado, desarrollado y operado por **[NOMBRE COMPLETO]** (en adelante, "el responsable"). Lo usa **una sola persona**: el propio responsable. No está disponible al público, no admite registro de usuarios y no se comercializa.

## 2. Datos de Google a los que accede Luca

Luca usa la API de Google Drive con un único permiso:

| Permiso (scope) | Para qué se usa |
| --- | --- |
| `https://www.googleapis.com/auth/drive.file` | Crear, leer y actualizar **solo los archivos que la propia aplicación crea** en la carpeta `Luca/` del Drive del responsable. Hoy se usa para guardar copias de seguridad cifradas. |

Con este permiso, Luca **no puede ver, leer ni modificar ningún otro archivo** del Google Drive del usuario.

Si en el futuro Luca necesita otros permisos de Google (por ejemplo, Calendar o Gmail), esta política se actualizará **antes** de solicitarlos, indicando el permiso y su finalidad.

## 3. Cómo se usan los datos

- Los archivos que Luca crea en Drive son copias de seguridad de su propia base de datos y configuración. **Están cifradas antes de salir del servidor**, así que Google no puede leer su contenido.
- Los datos solo se usan para prestarle el servicio al propio responsable.
- **No se venden, no se comparten con terceros y no se usan para publicidad**, perfiles comerciales ni para entrenar modelos de inteligencia artificial.

## 4. Uso limitado de los datos de Google

El uso y la transferencia a cualquier otra aplicación de la información recibida de las API de Google cumplen la [Política de datos de usuario de los servicios de API de Google](https://developers.google.com/terms/api-services-user-data-policy), incluidos sus requisitos de **Uso limitado** (*Limited Use*).

## 5. Almacenamiento y seguridad

- Luca corre en un servidor privado controlado por el responsable. No expone puertos a internet: solo es accesible por una red privada (Tailscale).
- Las credenciales de acceso (tokens OAuth) se guardan en el servidor como variables de entorno, fuera del código fuente y de cualquier repositorio.
- Las copias de seguridad se cifran con [restic](https://restic.net) antes de subirse a Google Drive.

## 6. Conservación y eliminación

- Las copias de seguridad se conservan con rotación automática: 7 diarias, 4 semanales y 6 mensuales. Las más antiguas se eliminan solas.
- Para borrar todos los datos basta con eliminar la carpeta `Luca/` de Google Drive.
- Para revocar el acceso de Luca a Google en cualquier momento: <https://myaccount.google.com/permissions>.

## 7. Marco legal

El tratamiento de datos personales se rige por la Ley Estatutaria 1581 de 2012 de Colombia y sus normas reglamentarias. Como el responsable y el único titular de los datos son la misma persona, no hay transferencia de datos a terceros.

## 8. Contacto

Para cualquier consulta sobre esta política: juanjosemayorquincabrera@gmail.com.

## 9. Cambios

Cualquier cambio a esta política se publica en esta misma página, actualizando la fecha de "Última actualización".
