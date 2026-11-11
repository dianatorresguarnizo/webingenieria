# Laboratorio: maquetación web y diseño adaptable

Proyecto demostrativo basado en la presentación **Clase 5 – Maquetación web y diseño adaptable** de Ingeniería Web.

## Cómo abrirlo

1. Descomprime la carpeta.
2. Abre la carpeta `Ejemplos_Maquetacion_Ingenieria_Web` en Visual Studio Code.
3. Abre `index.html` con **Live Server** (o directamente en el navegador).
4. Navega por los ejemplos desde el menú.
5. Utiliza DevTools > Toggle device toolbar para variar el ancho de pantalla.

**No necesitas XAMPP, PHP, JavaScript ni una base de datos.** Flexbox, CSS Grid y los ejemplos responsive funcionan sin conexión. Bootstrap y Tailwind necesitan Internet, porque cargan bibliotecas desde CDN.

## Mapa de ejemplos con las diapositivas

| Archivo | Diapositivas | Conceptos |
|---|---|---|
| `flexbox.html` | 5, 6, 7 | `.menu`, `.acciones`, `justify-content`, `align-items`, `gap`, `flex-wrap` |
| `grid.html` | 8, 9, 10 | `.galeria`, `.tarjetas-auto`, `repeat`, `1fr`, `auto-fit`, `minmax` |
| `responsive.html` | 11, 12, 13, 14, 15 | `viewport`, imágenes flexibles, `@media`, mobile-first |
| `bootstrap.html` | 16, 17, 19 | `.container`, `.row`, `.col-12`, `.col-md-6` |
| `tailwind.html` | 16, 18, 19 | `grid-cols-1`, `md:grid-cols-2`, `lg:grid-cols-3` |

Todo el CSS nativo se encuentra en `css/estilos.css` y está comentado por diapositiva. Para Bootstrap y Tailwind se mantienen los ejemplos de clases que aparecen en la presentación; se añaden los CDN necesarios para que produzcan estilos reales en el navegador.

## Ejercicios en vivo recomendados

1. **Flexbox:** en `.acciones`, cambiar `justify-content: center` por `space-between`; observar la diferencia.
2. **Grid:** en `.galeria`, cambiar `repeat(3,1fr)` por `repeat(2,1fr)`; contar columnas.
3. **Auto-fit:** reducir el ancho de la ventana; comprobar cómo se reacomodan las tarjetas.
4. **Media query:** modificar el valor `768px` a `900px`; observar cuándo cambian las columnas.
5. **Mobile-first:** probar anchos de 390, 800 y 1200 píxeles para comparar 1, 2 y 3 columnas.
6. **Frameworks:** abrir Bootstrap o Tailwind con internet y comparar cuántas reglas CSS propias es necesario escribir.

## Práctica de 40 minutos (igual que la presentación)

- 05 min: elegir una página HTML del proyecto del equipo.
- 10 min: usar Flexbox para menú o botones.
- 10 min: usar Grid para una sección de tarjetas.
- 10 min: aplicar mobile-first y media queries y comprobar en DevTools.
- 05 min: hacer commit y push; guardar capturas de móvil y escritorio.

**Evidencia:** enlace al repositorio de GitHub y dos capturas de la misma página con diferentes anchos.

## Nota para el docente

El ejemplo de tres columnas de la diapositiva 8 se complementa con una media query en pantallas muy estrechas para evitar tarjetas demasiado apretadas. El ejemplo auto-fit usa `min(100%,220px)` dentro de `minmax` como protección adicional contra el desbordamiento en contenedores excepcionalmente angostos. Estas pequeñas adaptaciones no cambian el concepto pedagógico mostrado.
