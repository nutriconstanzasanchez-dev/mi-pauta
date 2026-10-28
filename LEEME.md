# Mi pauta (app instalable)

Creada por Nta. Constanza (Demi) Sánchez · Instagram @nutridemi

## Qué contiene esta carpeta
- `index.html`: la app completa.
- `manifest.webmanifest` e `icons/`: nombre, colores e ícono para instalarla en el celular.
- `sw.js`: permite que funcione sin internet después de la primera vez.

No hay que instalar nada ni usar programas: es una página web estática.

## Publicar en Vercel con GitHub (sin código)
1. Entra a github.com, toca **New repository**, ponle el nombre `mi-pauta` y créalo.
2. En el repositorio nuevo toca **Add file → Upload files** y arrastra TODO el contenido de esta carpeta (index.html, manifest.webmanifest, sw.js y la carpeta icons). Toca **Commit changes**.
3. Entra a vercel.com con tu cuenta de GitHub y toca **Add New → Project**.
4. Elige el repositorio `mi-pauta` y toca **Import**.
5. En **Framework Preset** deja **Other**. No cambies nada más. Toca **Deploy**.
6. Al terminar, Vercel te da una dirección como `mi-pauta.vercel.app`. Esa es la que les mandas a tus pacientes.

## Cómo la instalan tus pacientes
- **Android (Chrome):** abren la dirección, van a la pestaña Mi pauta y tocan **Instalar Mi pauta** (o menú de tres puntos → Instalar app).
- **iPhone (Safari):** abren la dirección, tocan el botón Compartir → **Agregar a inicio**. Tiene que ser Safari.

## Actualizar la app después
Cuando haya una versión nueva, en tu repositorio de GitHub reemplaza `index.html` (Add file → Upload files, mismo nombre). Vercel la publica sola en un minuto. En `sw.js` cambia `mipauta-v1` por `mipauta-v2` si quieres forzar que todos reciban la actualización.

## Dirección propia (opcional)
En Vercel: Settings → Domains, y agregas por ejemplo `pauta.nutridemi.cl` si tienes ese dominio.

## Datos de las pacientes
Todo se guarda solo en el celular de cada paciente. Tú no ves nada ni se sube a ningún servidor. Si desinstalan la app o borran los datos del navegador, pierden su historial. Para mostrarte su avance en la consulta, abren la pestaña Mes.
