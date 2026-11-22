# KVM Variedades y más

Sitio web estático para publicar en GitHub Pages.

## Incluye
- Catálogo adaptable a celular y computadora.
- Búsqueda sin distinguir mayúsculas ni tildes.
- Filtros por categoría.
- Carrito y armado de pedido por WhatsApp.
- Panel local para agregar, editar, eliminar y activar/agotar productos.
- Cambio del número de WhatsApp y texto del logotipo.
- Importación y exportación de catálogo JSON.

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub.
2. Sube `index.html` a la raíz del repositorio.
3. Abre **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**.
5. Selecciona la rama `main` y la carpeta `/ (root)`, guarda.
6. Espera a que GitHub Pages publique el sitio y abre la dirección que te muestra.

## Configuración inicial
- El número inicial de WhatsApp es `50583761419`. Puedes cambiarlo desde Administración.
- El logotipo original está en `assets/logo-kvm.jpg` y aparece en la cabecera y la portada.
- No se incluyen productos ficticios: agrega tus productos, precios, existencias y fotografías desde Administración.
- Contraseña inicial del panel: `CAMBIAR-ESTA-CLAVE`. Cámbiala inmediatamente desde **Cambiar contraseña local**.

## Importante sobre seguridad y sincronización
Esta es una versión estática. Los productos, ajustes y contraseña se guardan en el almacenamiento local del navegador (`localStorage`). Eso significa:
- Los cambios solo aparecen en ese navegador y dispositivo.
- Los visitantes no comparten automáticamente un inventario actualizado.
- La contraseña está en el código del navegador y NO protege información sensible.
- No uses esta versión para guardar datos privados ni para gestionar pagos.

Para una tienda pública con panel realmente protegido y catálogo sincronizado entre dispositivos, hay que conectar un servicio backend (por ejemplo Supabase o Firebase), configurar autenticación y guardar los productos en una base de datos. GitHub Pages por sí solo no ofrece esa seguridad ni una base de datos.

## Logotipo
El logotipo original proporcionado se encuentra en `assets/logo-kvm.jpg`. Para sustituirlo, conserva ese nombre y esa ruta.

## Cambiar el logotipo desde Administración
Abre Administración, inicia sesión y en “Datos de la tienda” elige “Elegir imagen del dispositivo”. La imagen nueva se muestra en la cabecera y en la portada. Puedes restaurar el logo original cuando quieras. El cambio se guarda en el navegador actual; para publicarlo para todos los visitantes debes actualizar el sitio o conectar almacenamiento compartido.
