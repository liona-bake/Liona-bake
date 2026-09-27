# Liona.Bake

Sitio web de **Liona.Bake** — tortas saludables, cookies saludables, matcha ceremonial y pan de masa madre. Todo horneado artesanalmente, sin azúcar refinada, con ingredientes reales.

Página autocontenida en un solo archivo HTML (React 18 vía CDN + CSS embebido, sin build ni dependencias que instalar).

---

## 🌿 Productos

- **Tortas saludables** — endulzadas con dátiles y panela, sin harinas refinadas.
- **Cookies saludables** — sin gluten, sin azúcar, con avena, almendra y coco.
- **Matcha** — ceremonial grado A, importado de Japón.
- **Pan de masa madre** — fermentación lenta de 24 horas, corteza crujiente y miga alveolada.

---

## 🚀 Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (público para Pages gratis).
2. Sube el archivo `index.html` a la raíz del repositorio.
3. Ve a **Settings → Pages**.
4. En "Build and deployment", selecciona **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda. En unos minutos tu sitio estará disponible en:

```
https://<tu-usuario>.github.io/<nombre-del-repo>/
```

---

## 📞 Contacto

- **WhatsApp:** +57 (304) 391-5423
- **Email:** lioona.col@gmail.com
- **Instagram:** [@liona.bake](https://instagram.com/liona.bake)
- **TikTok:** [@liona.bake](https://tiktok.com/@liona.bake)
- **Horario:** Lun a Sáb · 8:00 a. m. - 6:00 p. m.

---

## 📝 Notas técnicas

- Todo el sitio vive en `index.html`: no hay que instalar nada ni correr `npm install`.
- El carrito y las reseñas se guardan en el navegador de cada visitante (`localStorage`), no en un servidor.
- Los pedidos se envían por WhatsApp al número configurado dentro del archivo (`CONFIG.WHATSAPP_NUMBER`).
- Para usar un dominio propio (como `liona.bake`), configúralo en **Settings → Pages → Custom domain**.
- El sitio es **mobile-first** y funciona correctamente en iOS (incluye `env(safe-area-inset-*)`) y Android.
- **Sin dependencias externas de CSS**: todo el diseño está embebido en el archivo, por lo que funciona incluso en redes que bloquean CDNs de estilos.
- React 18 se carga desde **jsDelivr** (`cdn.jsdelivr.net`), que funciona correctamente en redes colombianas.

---

## 🛠️ Configuración interna

Todos los datos editables están en el objeto `CONFIG` al inicio del `<script>` dentro de `index.html`:

```js
const CONFIG = {
  BUSINESS_NAME: "Liona.Bake",
  TAGLINE: "Horneado saludable, sabor que cuida.",
  WHATSAPP_NUMBER: "573043915423",
  WHATSAPP_DISPLAY: "+57 (304) 391-5423",
  INSTAGRAM_URL: "https://instagram.com/liona.bake",
  INSTAGRAM_HANDLE: "@liona.bake",
  TIKTOK_URL: "https://tiktok.com/@liona.bake",
  TIKTOK_HANDLE: "@liona.bake",
  EMAIL: "lioona.col@gmail.com",
  BUSINESS_HOURS: "Lun a Sáb · 8:00 a. m. - 6:00 p. m."
  // ...
};
```

---

## 🎯 Cómo subirlo

1. Abre tu repositorio `Liona-bake.github.io` en GitHub.
2. Toca **Add file → Create new file**.
3. Nombra el archivo `README.md`.
4. Pega el contenido de arriba.
5. Baja al final → **Commit changes**.

El README aparecerá automáticamente en la página principal del repo. 🌿
