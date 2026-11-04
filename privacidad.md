---
title: Política de privacidad de Luca
---

# Política de privacidad de Luca

**Última actualización:** 4 de noviembre de 2026

## 1. Qué es Luca

Luca es un asistente personal de uso privado, desarrollado y operado por **JUAN JOSÉ MAYORQUÍN CABRERA** (en adelante, "el responsable"). Lo usa **una sola persona**: el propio responsable. No está disponible al público, no admite registro de usuarios y no se comercializa.

## 2. Datos de Google a los que accede Luca

Luca usa las API de Google Drive y Google Calendar con estos permisos:

| Permiso (scope) | Para qué se usa |
| --- | --- |
| `https://www.googleapis.com/auth/drive.file` | Crear, leer y actualizar **solo los archivos que la propia aplicación crea** en la carpeta `Luca/` del Drive del responsable. Hoy se usa para guardar copias de seguridad cifradas. |
| `https://www.googleapis.com/auth/calendar.events` | **Leer** los eventos de dos calendarios del responsable (personal y universidad) para armar el resumen del día y avisarle a tiempo, y **crear o modificar** eventos en esos calendarios cuando el responsable se lo pide. Borrar un evento siempre requiere su confirmación. |

Con el permiso de Drive, Luca **no puede ver, leer ni modificar ningún otro archivo** del Google Drive del usuario. Con el de Calendar, Luca solo consulta los calendarios configurados, **nunca borra eventos por su cuenta** y no accede a la configuración ni a la lista de contactos del usuario.

Además, para calcular la hora de salida en días de oficina, Luca envía a la API de rutas de Google Maps (Routes API) el origen y el destino del trayecto. Esta consulta usa una clave de API del propio proyecto, no la cuenta de Google del usuario, y no se guarda el historial de ubicaciones.

Si en el futuro Luca necesita otros permisos de Google (por ejemplo, Gmail), esta política se actualizará **antes** de solicitarlos, indicando el permiso y su finalidad.

## 3. Cómo se usan los datos

- Los archivos que Luca crea en Drive son copias de seguridad de su propia base de datos y configuración. **Están cifradas antes de salir del servidor**, así que Google no puede leer su contenido.
- Los eventos del calendario se leen al momento de usarlos (resumen del día, planeación) y no se copian a otros servicios. Luca puede mencionarlos en sus mensajes privados al responsable por Telegram.
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
- Para borrar todos los datos basta con eliminar la carpeta `Luca/` de Google Drive. Los eventos del calendario siguen en Google Calendar y se gestionan desde allí.
- Para revocar el acceso de Luca a Google en cualquier momento: <https://myaccount.google.com/permissions>.

## 7. Marco legal

El tratamiento de datos personales se rige por la Ley Estatutaria 1581 de 2012 de Colombia y sus normas reglamentarias. Como el responsable y el único titular de los datos son la misma persona, no hay transferencia de datos a terceros.

## 8. Contacto

Para cualquier consulta sobre esta política: juanjosemayorquincabrera@gmail.com.

## 9. Cambios

Cualquier cambio a esta política se publica en esta misma página, actualizando la fecha de "Última actualización".
