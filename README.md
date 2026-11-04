# ComeQueTeCome

Primera versión de una PWA (aplicación web instalable) para organizar menús y listas de compra.

## Qué incluye
- Interfaz responsive para móvil y ordenador.
- Menú de siete días y cinco comidas configurables.
- Recetas de ejemplo con ingredientes para dos personas.
- Lista de compra agrupada por secciones y casillas para marcar.
- Presupuesto editable y supermercado Mercadona como referencia.
- Preferencias guardadas localmente en el dispositivo.
- Caché básica para volver a abrir la app sin conexión tras la primera visita.

## Cómo probarla en tu ordenador
Abre una terminal dentro de esta carpeta y ejecuta:
`python -m http.server 8000`
Después abre `http://localhost:8000`.

## Cómo publicarla gratis como web
1. Crea una cuenta en GitHub y un repositorio llamado `comequetecome`.
2. Sube todos los archivos de esta carpeta a la raíz del repositorio.
3. En Settings → Pages, selecciona Deploy from a branch y la rama `main` / root.
4. GitHub Pages te dará una dirección pública HTTPS.
5. Abre esa dirección en el móvil y usa “Añadir a pantalla de inicio” (iPhone: Compartir → Añadir a pantalla de inicio; Android: menú del navegador → Instalar app).

También se puede desplegar en Netlify o Vercel conectando el repositorio.

## Importante: alcance del prototipo
Esta primera versión es una demo funcional con recetas y precios no verificados. El presupuesto no calcula todavía precios reales de Mercadona ni conecta con su catálogo. Los datos se guardan en el almacenamiento local del navegador y no se sincronizan entre dispositivos. Para una versión multiusuario se necesitarán backend, cuentas, sincronización, gestión de perfiles y revisión de seguridad alimentaria.

La alergia al marisco requiere comprobar etiquetas, posibles trazas y contaminación cruzada. Ninguna app puede garantizar por sí sola que un producto comercial sea seguro.


Actualización nutricional: muestra estimaciones por persona de energía (kcal), proteínas, hidratos de carbono, grasas y fibra en las tarjetas del menú y del recetario. Son valores orientativos, no datos de laboratorio.
