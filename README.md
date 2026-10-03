---

## Estructura del proyecto

```text
Proyecto-Final/
├── index.html
├── style.css
├── .gitignore
└── README.md

Taller 1: HTML5 + CSS3 y Git/GitHub
Descripción del Taller 1
En el Taller 1 se desarrolló la estructura inicial de una página web utilizando HTML5 y CSS3.
Se aplicaron elementos semánticos de HTML5 para organizar correctamente el contenido de la página.
Estructura HTML
La página contiene los siguientes elementos principales:
- header
- nav
- main
- section
- footer
También se incorporaron:
- Una tabla con información ficticia.
- Un formulario.
- Una sección de información.
- Elementos de navegación.
Diseño CSS
Se creó el archivo style.css para aplicar los estilos visuales de la página.
Se trabajaron aspectos como:
- Tipografía.
- Colores.
- Márgenes.
- Espaciado.
- Bordes.
- Estilos de tablas.
- Estilos de formularios.
- Diseño de las diferentes secciones.
Control de versiones
Para el desarrollo colaborativo se utilizó Git y GitHub.
Se trabajó mediante ramas para separar los cambios realizados por cada integrante.
La rama utilizada por Jefferson fue:
dev/jefferson

La rama utilizada para los cambios de Juliza fue:
EstilosJuliza

Los cambios fueron registrados mediante commits y posteriormente integrados mediante Pull Requests.
Taller 2: Integración, Galería/Grid y resolución de conflictos
Objetivo
El objetivo del Taller 2 fue integrar los cambios realizados por los integrantes del proyecto, incorporar una sección de Galería utilizando CSS Grid, mejorar la adaptación de la página para dispositivos pequeños y resolver un conflicto durante la integración de ramas.
Galería de proyectos
Se agregó una nueva sección denominada:
Galería de proyectos

La galería está compuesta por cuatro elementos:
1. Proyecto 1 - Desarrollo de estructura HTML5.
2. Proyecto 2 - Diseño y estilos utilizando CSS3.
3. Proyecto 3 - Trabajo colaborativo utilizando Git.
4. Proyecto 4 - Control de versiones utilizando GitHub.
Para organizar los elementos de la galería se utilizó CSS Grid.
Estructura HTML de la galería
<div class="galeria-grid">

    <div class="galeria-item">
        <h3>Proyecto 1</h3>
        <p>Desarrollo de estructura HTML5.</p>
    </div>

    <div class="galeria-item">
        <h3>Proyecto 2</h3>
        <p>Diseño y estilos utilizando CSS3.</p>
    </div>

    <div class="galeria-item">
        <h3>Proyecto 3</h3>
        <p>Trabajo colaborativo utilizando Git.</p>
    </div>

    <div class="galeria-item">
        <h3>Proyecto 4</h3>
        <p>Control de versiones utilizando GitHub.</p>
    </div>

</div>

Estilos de la Galería
Para la galería se utilizó CSS Grid con dos columnas en pantallas de tamaño normal.
.galeria-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    margin-top: 20px;
}

.galeria-item {
    background-color: #f4f6f8;
    border: 1px solid #dddddd;
    border-radius: 8px;
    padding: 20px;
    text-align: center;
}

.galeria-item h3 {
    color: #1d4ed8;
    margin-bottom: 10px;
}

.galeria-item p {
    margin: 0;
}

Diseño Responsive
Se agregó una regla @media para adaptar la página a dispositivos con pantallas pequeñas.
Cuando el ancho de pantalla es menor o igual a 600 píxeles, la galería pasa de dos columnas a una sola columna.
@media (max-width: 600px) {

    .galeria-grid {
        grid-template-columns: 1fr;
    }

}

También se aplicaron estilos responsive a los elementos del formulario para facilitar su visualización en dispositivos pequeños.
Resolución del conflicto
Generación del conflicto
Durante la integración de los cambios de las diferentes ramas se produjo un conflicto en el archivo:
style.css

El conflicto ocurrió al intentar integrar los cambios de la rama de Juliza con los cambios realizados en la rama de Jefferson.
Para realizar la integración se utilizaron los siguientes comandos:
git fetch origin
git merge origin/EstilosJuliza

Git informó que existía un conflicto en el archivo style.css.
Solución del conflicto
Se revisaron manualmente las diferencias mostradas por Git.
Se conservaron los estilos necesarios del proyecto y se integraron los cambios correspondientes a la galería y al diseño responsive.
Después de resolver manualmente el conflicto, se agregaron los archivos modificados al área de preparación:
git add index.html style.css

Posteriormente se creó un commit específico para registrar la resolución del conflicto:
git commit -m "fix: resolver conflicto en estilos de tabla"

Finalmente, los cambios fueron enviados a GitHub:
git push origin dev/jefferson

Pull Request
Después de resolver el conflicto y subir los cambios a GitHub, se creó un Pull Request desde:
dev/jefferson

hacia:
main

El Pull Request fue revisado por la integrante del proyecto.
Después de la revisión y aprobación, el Pull Request fue fusionado con la rama principal main.
Actualización de la rama principal
Después de realizar la integración en GitHub, se actualizó la rama principal local utilizando:
git switch main

y:
git pull origin main

De esta manera se obtuvo localmente la versión actualizada del proyecto.
Finalmente, se verificó el estado del repositorio:
git status

El repositorio quedó actualizado y sin cambios pendientes.
Resultado final
Después de completar los Talleres 1 y 2, el proyecto cuenta con:
- Estructura HTML5.
- Diseño mediante CSS3.
- Navegación.
- Tabla de información.
- Formulario.
- Sección informativa.
- Galería de proyectos.
- Diseño mediante CSS Grid.
- Diseño responsive.
- Trabajo colaborativo mediante Git y GitHub.
- Uso de ramas.
- Uso de commits.
- Pull Request.
- Revisión de cambios.
- Resolución de un conflicto de Git.
- Integración final en la rama main.
Evidencias
Evidencia del conflicto
La siguiente imagen muestra el conflicto generado durante la integración de las ramas:
 
Evidencia de la revisión del Pull Request
La siguiente imagen muestra la revisión y aprobación del Pull Request:
 
Evidencia del Pull Request fusionado
La siguiente imagen muestra el Pull Request después de ser fusionado con la rama main:
 
Evidencia del estado final
La siguiente imagen muestra el estado final del repositorio después de actualizar la rama main:
 
Conclusión
El desarrollo de este proyecto permitió aplicar conocimientos de HTML5 y CSS3 junto con herramientas de control de versiones como Git y GitHub.
El trabajo colaborativo permitió utilizar ramas independientes, realizar commits, crear Pull Requests, revisar cambios y resolver un conflicto de integración.
Como resultado, se obtuvo una página web funcional, organizada, responsive y con un historial de trabajo colaborativo mediante Git.