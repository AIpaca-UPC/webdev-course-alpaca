# 🧪 Plantillas de las actividades prácticas

En esta guía encontrarás el código inicial de las cinco actividades del curso **Fundamentos de Desarrollo Web**. Cada plantilla está pensada para que puedas ejecutarla, modificarla y observar qué cambia en el navegador.

## Cómo utilizar las plantillas

1. Abre el editor indicado en la actividad.
2. Copia el código HTML en el panel **HTML**.
3. Si la actividad incluye CSS, copia ese código en el panel **CSS**.
4. Ejecuta la vista previa y realiza el reto propuesto.
5. Modifica el código: equivocarse y probar cambios también forma parte del aprendizaje.

| Editor | Cómo pegar el código |
|---|---|
| [CodePen](https://codepen.io/pen/) | Pega HTML y CSS en sus paneles correspondientes. |
| [JSFiddle](https://jsfiddle.net/) | Pega el HTML y CSS en sus paneles y pulsa **Run**. |
| [Replit](https://replit.com/) | Crea los archivos indicados y pega cada bloque en su archivo. |

> **Importante:** los enlaces de los editores abren un espacio de trabajo. El código inicial está en esta guía; cópialo en el editor para comenzar.

---

<a id="leccion-1"></a>
## Lección 1. Explorar sitios web

**Editor:** [CodePen](https://codepen.io/pen/)  
**Objetivo:** reconocer que HTML organiza el contenido y CSS controla su presentación visual.

### HTML

~~~html
<header class="hero">
  <p class="eyebrow">MI PRIMERA EXPLORACIÓN</p>
  <h1>Bienvenido a la web</h1>
  <p>Una página web combina contenido y diseño para comunicar ideas.</p>
</header>

<main class="container">
  <section class="card">
    <h2>HTML: el contenido</h2>
    <p>HTML permite organizar títulos, párrafos, imágenes, enlaces y otras partes de una página.</p>
  </section>

  <section class="card card-highlight">
    <h2>CSS: la apariencia</h2>
    <p>CSS permite cambiar colores, tamaños, espacios, bordes y la distribución de los elementos.</p>
  </section>
</main>

<footer>
  <p>Mi primera exploración del desarrollo web</p>
</footer>
~~~

### CSS

~~~css
body {
  margin: 0;
  font-family: Arial, sans-serif;
  color: #243047;
  background: #f2f5fa;
}

.hero {
  padding: 48px 20px;
  text-align: center;
  color: white;
  background: #3157a4;
}

.eyebrow {
  letter-spacing: 2px;
  font-size: 12px;
  font-weight: bold;
}

.container {
  width: min(850px, 90%);
  margin: 30px auto;
  display: grid;
  gap: 18px;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
}

.card {
  padding: 24px;
  background: white;
  border-radius: 14px;
  box-shadow: 0 5px 18px #172b4d14;
}

.card-highlight {
  border-top: 5px solid #36a58b;
}

footer {
  padding: 18px;
  text-align: center;
  color: #667085;
}
~~~

**Reto:** cambia el título, modifica el color del encabezado y observa qué parte del código controla cada cambio.

---

<a id="leccion-2"></a>
## Lección 2. Primera página HTML

**Editor:** [CodePen](https://codepen.io/pen/)  
**Objetivo:** reconocer los encabezados, párrafos, etiquetas y atributos HTML.

### Estructura completa de un documento HTML

Este ejemplo muestra dónde se ubican las etiquetas **head** y **body** en un archivo HTML. Puedes guardarlo como **index.html** si trabajas en un editor de archivos.

~~~html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi primera página</title>
</head>
<body>
  <h1>¡Hola, mundo!</h1>
  <h2>Mi primera página web</h2>
  <p>Estoy aprendiendo a crear páginas con HTML.</p>
  <p title="Este es un atributo HTML">Pasa el cursor sobre este párrafo.</p>
</body>
</html>
~~~

### Código para el panel HTML de CodePen

CodePen ya prepara la estructura externa del documento. Por eso, en su panel HTML pega solamente el contenido que iría dentro de **body**.

~~~html
<h1>¡Hola, mundo!</h1>

<h2>Sobre mí</h2>
<p>Estoy aprendiendo a crear mi primera página web.</p>

<h2>Mis temas favoritos</h2>
<p>Me interesa la tecnología, el diseño y la creatividad.</p>

<p title="Este texto contiene un atributo title">
  Coloca el cursor sobre este párrafo.
</p>
~~~

**Reto:** agrega un tercer encabezado h2, escribe un nuevo párrafo y cambia el texto del atributo title.

---

<a id="leccion-3"></a>
## Lección 3. Añadir imágenes, listas y enlaces

**Editor:** [JSFiddle](https://jsfiddle.net/)  
**Objetivo:** complementar una página con listas, imágenes y enlaces.

### HTML

~~~html
<h1>Mis lugares favoritos</h1>
<p>Estos son algunos lugares que me gustaría conocer.</p>

<h2>Mi lista de destinos</h2>
<ul>
  <li>Montañas</li>
  <li>Playas</li>
  <li>Ciudades históricas</li>
</ul>

<h2>Una imagen de ejemplo</h2>
<img
  src="https://placehold.co/640x360?text=Mi+imagen"
  alt="Imagen de ejemplo para la actividad"
>

<h2>Aprende más</h2>
<p>
  Visita la
  <a href="https://developer.mozilla.org/es/docs/Web/HTML" target="_blank" rel="noopener noreferrer">
    documentación de HTML en MDN
  </a>.
</p>
~~~

### CSS

~~~css
body {
  max-width: 760px;
  margin: 35px auto;
  padding: 0 20px;
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #263238;
}

h1, h2 {
  color: #245b82;
}

img {
  display: block;
  width: 100%;
  max-width: 640px;
  height: auto;
  border-radius: 12px;
}

a {
  color: #087f8c;
  font-weight: bold;
}
~~~

**Reto:** agrega dos elementos a la lista, cambia el texto alternativo de la imagen y crea un enlace a otro sitio web.

---

<a id="leccion-4"></a>
## Lección 4. Dar estilo a la página con CSS

**Editor:** [CodePen](https://codepen.io/pen/)  
**Objetivo:** aplicar colores, tipografías, márgenes, bordes y selectores CSS.

### HTML

~~~html
<main class="page">
  <p class="tag">DISEÑO WEB</p>
  <h1>Haz que tu página destaque</h1>
  <p class="intro">Con CSS puedes transformar una estructura sencilla en una página agradable y fácil de leer.</p>

  <section class="features">
    <article class="feature">
      <h2>Colores</h2>
      <p>Elige una paleta que comunique tu idea.</p>
    </article>

    <article class="feature">
      <h2>Tipografía</h2>
      <p>Organiza los textos con tamaños y pesos adecuados.</p>
    </article>

    <article class="feature">
      <h2>Espaciado</h2>
      <p>Utiliza márgenes y rellenos para dar aire al contenido.</p>
    </article>
  </section>
</main>
~~~

### CSS

~~~css
:root {
  --primary: #3157a4;
  --accent: #36a58b;
  --background: #f3f6fb;
  --text: #243047;
}

body {
  margin: 0;
  padding: 35px 18px;
  font-family: Arial, sans-serif;
  color: var(--text);
  background: var(--background);
}

.page {
  max-width: 900px;
  margin: auto;
}

.tag {
  color: var(--accent);
  font-size: 13px;
  font-weight: bold;
  letter-spacing: 2px;
}

h1 {
  color: var(--primary);
  font-size: clamp(30px, 5vw, 46px);
}

.intro {
  max-width: 650px;
  line-height: 1.7;
}

.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(190px, 1fr));
  gap: 16px;
  margin-top: 28px;
}

.feature {
  padding: 22px;
  background: white;
  border-radius: 14px;
  border-bottom: 4px solid var(--accent);
  box-shadow: 0 5px 18px #172b4d12;
}
~~~

**Reto:** cambia los valores de primary, accent y background. Después modifica el tamaño del título y el borde de las tarjetas.

---

<a id="leccion-5"></a>
## Lección 5. Crear una página de perfil personal

**Editor:** [Replit](https://replit.com/)  
**Objetivo:** combinar HTML y CSS para construir una página de perfil sencilla.

En Replit crea dos archivos: **index.html** y **style.css**.

### Archivo index.html

~~~html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi perfil</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <main class="profile">
    <img
      class="avatar"
      src="https://placehold.co/180x180?text=Foto"
      alt="Imagen de perfil de ejemplo"
    >

    <p class="tag">MI PÁGINA PERSONAL</p>
    <h1>¡Hola! Soy Alex</h1>
    <p class="description">
      Soy estudiante y estoy aprendiendo desarrollo web.
      Me gusta descubrir cosas nuevas y crear proyectos.
    </p>

    <section class="interests">
      <h2>Mis intereses</h2>
      <ul>
        <li>Tecnología</li>
        <li>Música</li>
        <li>Deportes</li>
      </ul>
    </section>

    <a class="button" href="mailto:correo@ejemplo.com">Contáctame</a>
  </main>
</body>
</html>
~~~

### Archivo style.css

~~~css
body {
  min-height: 100vh;
  margin: 0;
  padding: 30px 16px;
  display: grid;
  place-items: center;
  font-family: Arial, sans-serif;
  color: #243047;
  background: #edf2fa;
}

.profile {
  width: min(100%, 440px);
  box-sizing: border-box;
  padding: 32px;
  text-align: center;
  background: white;
  border-radius: 20px;
  box-shadow: 0 10px 35px #172b4d18;
}

.avatar {
  width: 120px;
  height: 120px;
  object-fit: cover;
  border-radius: 50%;
  border: 5px solid #dce8fb;
}

.tag {
  margin-top: 22px;
  color: #36a58b;
  font-size: 12px;
  font-weight: bold;
  letter-spacing: 2px;
}

h1 {
  margin-bottom: 10px;
  color: #3157a4;
}

.description {
  line-height: 1.6;
}

.interests {
  margin: 24px 0;
  padding: 16px;
  text-align: left;
  background: #f3f6fb;
  border-radius: 12px;
}

.button {
  display: inline-block;
  padding: 12px 22px;
  color: white;
  text-decoration: none;
  background: #3157a4;
  border-radius: 999px;
}

.button:hover {
  background: #243f79;
}
~~~

**Reto:** cambia el nombre, la descripción, la imagen y los intereses. Personaliza también los colores de tu perfil.

> **Privacidad:** utiliza información ficticia o datos que tengas autorización para compartir. No publiques tu dirección, teléfono ni información personal sensible.
