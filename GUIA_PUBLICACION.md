# WappControl AI — Paquete inicial gratuito

## Qué incluye
- `index.html`: prototipo web funcional para registrar clientes en el navegador, buscar y filtrar, actualizar estados, preparar mensajes de WhatsApp y exportar/importar copias.
- `GUIA_PUBLICACION.md`: pasos para probarlo y publicarlo gratis como página estática.
- `TEXTOS_COMERCIALES.md`: borradores de presentación y oferta.
- `ROADMAP.md`: qué falta para convertirlo en un producto SaaS multiusuario.

## Importante antes de vender
Esta versión guarda datos en el navegador del dispositivo. No tiene inicio de sesión, sincronización, base de datos compartida, aislamiento de clientes por negocio, ni envío automático por WhatsApp. No la vendas como plataforma multiusuario terminada. Primero valida el prototipo y después implementa autenticación, base de datos, seguridad, privacidad y las integraciones correspondientes.

## Probar en tu computadora
1. Descomprimí el ZIP en una carpeta.
2. Abrí `index.html` con Chrome, Edge o Firefox.
3. Agregá un cliente de prueba.
4. Probá búsqueda, edición, estados, plantillas, exportación CSV y copia JSON.
5. Los datos quedan en el navegador actual. No uses información sensible real en una demo pública.

## Publicación estática gratuita con GitHub Pages
1. Creá una cuenta en GitHub si no tenés una.
2. Creá un repositorio nuevo, por ejemplo `wappcontrol-ai`.
3. Si elegís que sea público, recordá que el código será visible. No subas datos de clientes ni claves.
4. Subí `index.html` a la raíz del repositorio.
5. Abrí Settings → Pages.
6. En Build and deployment, elegí Deploy from a branch; rama `main`, carpeta `/(root)` y guardá.
7. Esperá a que aparezca la URL publicada en esa sección.
8. Abrí la URL desde una ventana privada y comprobá que cargue.
9. La web estática no agrega cuentas, base de datos ni sincronización. Cada visitante tendrá sus propios datos locales en su navegador.

La disponibilidad y las condiciones de los planes gratuitos pueden cambiar; comprobá los límites actuales del proveedor antes de depender de ellos.

## Próxima etapa para un SaaS real
1. Definir cuentas de usuario y recuperación de contraseña.
2. Crear una base de datos con permisos por usuario/negocio.
3. Activar reglas de seguridad en el servidor/base de datos; nunca confiar solo en filtros del navegador.
4. Añadir pruebas para asegurar que un negocio no pueda ver datos de otro.
5. Crear política de privacidad, términos de uso y procedimiento para borrar/exportar datos.
6. Evaluar integración oficial con WhatsApp Business Platform y sus condiciones/costos actuales.
7. Añadir gestión de planes y cobros solo después de probar seguridad y funcionamiento.
8. No poner claves privadas, secretos ni tokens en `index.html` ni en repositorios públicos.
