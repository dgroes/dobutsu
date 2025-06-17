## C01: Importar Tailwind
Luego de instalar Tailwind CSS, será improtante importar el `global.css` que está dentro de la ruta `src/styles` que se creó cuando se instaló Tailwind. Entonces dentro de el `index.astro` deberia estar la importación: `import "../styles/global.css";` para que Astro reconozca Tailwind.

## C02: Añadir Tipografía
Para añadir una tipografia se deberá hacer dentro del `global.css` y además añadir el fichero de tipografía en `public/fonst`. Por mejor rendimiento la mejor exteción sería una con `.woff2`.

Luego de agregar el fichero de la tipográfia será importante llamarla para su uso dentro de `global.css`, aquí un ejemplo:
```css
@font-face {
  font-family: "GeneralSans";
  src: url("/fonts/GeneralSans-Medium.woff2") format("woff2");
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}```
