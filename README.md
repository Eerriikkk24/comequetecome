# ComeQueTeCome

Primera versión de una PWA (aplicación web instalable) para organizar menús y listas de compra.

## Qué incluye
- Interfaz responsive para móvil y ordenador.
- Menú de siete días y cinco comidas configurables.
- Recetas de ejemplo con ingredientes para dos personas.
- Lista de compra agrupada por secciones y casillas para marcar.
- Presupuesto editable.
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
Esta primera versión es una demo funcional con recetas y precios no verificados. El presupuesto no calcula todavía precios reales de supermercados ni conecta con catálogos de supermercados. Los datos se guardan en el almacenamiento local del navegador y no se sincronizan entre dispositivos. Para una versión multiusuario se necesitarán backend, cuentas, sincronización, gestión de perfiles y revisión de seguridad alimentaria.

La alergia al marisco requiere comprobar etiquetas, posibles trazas y contaminación cruzada. Ninguna app puede garantizar por sí sola que un producto comercial sea seguro.


Actualización nutricional: muestra estimaciones por persona de energía (kcal), proteínas, hidratos de carbono, grasas y fibra en las tarjetas del menú y del recetario. Son valores orientativos, no datos de laboratorio.


## Novedades de esta versión
- Recetario ampliado con nuevas ideas de desayuno, tentempiés, comidas y cenas.
- Objetivo calórico diario conjunto editable desde Preferencias.
- Resumen de calorías estimadas para los dos en cada día del menú.
- Las recetas de comida y cena se plantean para dos raciones iguales.
- Se ha actualizado la caché de la PWA para que los dispositivos reciban esta versión.
- Las cifras nutricionales son aproximadas; revisad etiquetas y alérgenos de cada producto.


### Ajuste del objetivo calórico
- El objetivo conjunto acepta valores exactos, por ejemplo 1500 kcal (pasos de 1 kcal).
- El resumen diario compara el objetivo conjunto con las calorías estimadas de las dos raciones.
- Las tarjetas de receta siguen mostrando kcal por persona.


## Lista de compra y precios (v6)
La lista suma ingredientes de toda la semana, calcula cantidades, estima envases completos y coste por producto, total y comparación con presupuesto. **Los precios precargados son ejemplos orientativos, no precios actuales verificados de ningún supermercado.** No hay consulta en vivo ni API externa. Los productos por peso/unidad son aproximados; revisar precios reales, alérgenos y trazas en tienda.


## Presupuesto automático (v7)
Al generar la semana o guardar presupuesto, se busca una combinación de recetas de menor coste semanal estimado, considerando envases enteros y cantidades ajustadas al objetivo calórico conjunto. Es una heurística, no garantiza el óptimo ni cumplir un presupuesto imposible. Los precios son referencias ilustrativas, NO precios actuales verificados. Comprueba la compra real y las alergias.
