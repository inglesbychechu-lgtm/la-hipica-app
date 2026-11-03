# La Hípica · Comandas

App de gestión de sala (mesas, comandas, cobros, carta, ventas e historial).

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub (por ejemplo `hipica-comandas`).
2. Sube el contenido de este zip a la raíz del repositorio (`index.html`, `config.js`, `.nojekyll`).
3. En el repositorio: Settings → Pages → Source: "Deploy from a branch" → rama `main`, carpeta `/ (root)` → Save.
4. En un par de minutos la app estará en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Dónde se guardan los datos
- **Por defecto (config.js en null):** los datos se guardan en el navegador de cada dispositivo. No se sincronizan entre móviles y tablets. Sirve para probar la app.
- **Con sincronización (Firebase):**
  1. Crea un proyecto en https://console.firebase.google.com y añade una app web.
  2. Activa Firestore Database.
  3. Pega el `firebaseConfig` en `config.js` (sustituye el `null`).
  4. En Firestore → Rules, restringe el acceso. Con reglas abiertas cualquiera que conozca la dirección podría leer y borrar datos. Lo ideal es añadir inicio de sesión antes de usarla en el restaurante.

## Primer uso
Abre la app. Si no hay datos, pulsa "Cargar datos de demostración" y después "Crear las 4 secciones". La carta de La Hípica se carga sola.

## Icono
La app incluye icono (herradura dorada con cubiertos), favicon y `manifest.json`. En el móvil puedes usar "Añadir a pantalla de inicio" y se abrirá como una app, con este icono.
