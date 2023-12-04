# SVG (Scalable Vector Graphics) è un formato di immagine basato su XML per la grafica vettoriale. Offre diversi vantaggi, tra cui la scalabilità senza perdita di qualità e la possibilità di essere manipolato tramite CSS e JavaScript. Ecco una panoramica dei tag SVG più importanti con esempi pratici:

## 1. <svg>
Il tag <svg> è il contenitore per ogni grafica SVG. Definisce l'area di lavoro o il viewport dell'SVG.

xml
Copy code
<svg width="100" height="100">
  <!-- Altri elementi SVG qui -->
</svg>
2. <circle>
Crea un cerchio. Gli attributi principali includono cx (coordinata x del centro), cy (coordinata y del centro) e r (raggio).

xml
Copy code
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
3. <rect>
Crea un rettangolo. Gli attributi principali sono x, y, width, height, e opzionalmente rx e ry per angoli arrotondati.

xml
Copy code
<svg width="100" height="100">
  <rect x="10" y="10" width="80" height="80" fill="blue" />
</svg>
4. <line>
Crea una linea. Richiede gli attributi x1, y1 (coordinate di inizio) e x2, y2 (coordinate di fine).

xml
Copy code
<svg width="100" height="100">
  <line x1="0" y1="0" x2="100" y2="100" stroke="black" />
</svg>
5. <polyline>
Crea una serie di linee connesse. L'attributo points è una lista di coordinate.

xml
Copy code
<svg width="100" height="100">
  <polyline points="20,20 40,25 60,40 80,120 120,140" stroke="black" fill="none"/>
</svg>
6. <polygon>
Simile a <polyline>, ma crea una forma chiusa. Anche qui, l'attributo points è usato per le coordinate.

xml
Copy code
<svg width="100" height="100">
  <polygon points="50,0 100,100 0,100" fill="#cccccc" stroke="#000000" />
</svg>
7. <path>
Il tag più potente e flessibile in SVG per creare percorsi complessi. Utilizza l'attributo d per definire il percorso.

xml
Copy code
<svg width="100" height="100">
  <path d="M10 10 H 90 V 90 H 10 L 10 10" fill="transparent" stroke="black"/>
</svg>
8. <text>
Permette di inserire testo. Gli attributi x e y determinano la posizione.

xml
Copy code
<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="20" fill="blue">Ciao!</text>
</svg>
9. <g>
Usato per raggruppare elementi SVG e applicare trasformazioni o stili a tutto il gruppo.

xml
Copy code
<svg width="100" height="100">
  <g fill="red">
    <circle cx="50" cy="50" r="40" />
    <text x="40" y="55">Hi</text>
  </g>
</svg>