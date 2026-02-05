# ASIX1_0373_AE1b_Apuntes

## Índice
1. **[GitHub](#id1)**
2. **[Git](#id2)**
3. **[Markdown](#id3)**
4. **[HTML](#id4)**
5. **[CSS](#id5)**

<div id='id1' />

---

## GitHub

<p align="center">
	<img src="img/github-logo.jpg" alt="GitHub logo" style="max-width:360px; width:60%; height:auto;">
</p>

GitHub es una plataforma en la nube que se utiliza para alojar proyectos de software, permitiendo a los desarrolladores colaborar, compartir y gestionar cambios en el código de forma remota.

### Crear un repositorio

En clase creamos una cuenta de GitHub (algunos ya la teníamos de SMX). Para crear un repositorio:

1. Acceder al menú de repositorios (arriba a la izquierda)
2. Hacer clic en "New repository"
3. Completar la información solicitada:
   - **Nombre del repositorio**: Identificador único del proyecto
   - **Descripción**: Breve explicación del contenido
   - **Visibilidad**: Público o privado
   - **README**: Se recomienda añadirlo desde el inicio para facilitar el trabajo posterior

Una vez todo escrito y seleccionado, solamente quedará darle a crear el repositorio, así ya nos aparecerá el repositorio en nuestra cuenta.

---
<div id='id2' />

## Git


Git se utiliza principalmente para gestionar el historial de cambios en archivos de código fuente, permitiendo que múltiples desarrolladores colaboren en un proyecto de manera simultánea.
En nuestro caso lo utilizaremos para poder hacer todos los commits que vayamos haciendo en el Visual Studio Code.

### Instalación

Antes de usar Git, es necesario instalarlo para que funcione en la línea de comandos (cmd).

Una vez instalado, los comandos que se tendrán que utilizar serán los siguientes:

### Comandos principales

- **`git clone [URL]`**: Clona un repositorio remoto creando una carpeta local con todo su contenido
````bash
  git clone https://github.com/usuario/repositorio.git
````

- **`git init`**: Inicializa un repositorio Git en la carpeta actual
````bash
  git init
````

- **`git add .`**: Añade todos los cambios (archivos nuevos, modificados o eliminados) al área de preparación
````bash
  git add .
````

- **`git commit -m "mensaje"`**: Crea un commit con los cambios preparados y un mensaje descriptivo
````bash
  git commit -m "Añadida sección de GitHub"
````

- **`git push origin main`**: Envía los commits locales al repositorio remoto en GitHub
````bash
  git push origin main
````

### Flujo de trabajo

1. Realizar cambios en los archivos
2. `git add .` para preparar los cambios
3. `git commit -m "descripción"` para guardar los cambios localmente
4. `git push origin main` para sincronizar con GitHub

Hecho todo esto, ya tendrás el commit enviado de tu local al GitHub.

---
<div id='id3' />

## Markdown

Markdown es un lenguaje de marcas ligero que permite crear documentos con formato de manera sencilla y legible. Se usa mucho en archivos README, documentación y foros.

Ahora haré una explicación básica con sus respectivos ejemplos de etiquetas comunes:
Encabezados

Se utilizan almohadillas `#` al inicio de la línea, seguidas de un espacio:
````markdown
# Encabezado nivel 1 (h1)
## Encabezado nivel 2 (h2)
### Encabezado nivel 3 (h3)
#### Encabezado nivel 4 (h4)
##### Encabezado nivel 5 (h5)
###### Encabezado nivel 6 (h6)
````

Cuantas más almohadillas (máximo 6), más pequeño será el encabezado.

### Énfasis de texto

**Negrita**: Se puede usar doble asterisco `**texto**` o doble guion bajo `__texto__`
- Ejemplo: **negrita**

*Cursiva*: Se usa un asterisco `*texto*` o un guion bajo `_texto_`
- Ejemplo: *cursiva*

***Negrita y cursiva***: Tres asteriscos `***texto***` o combinación `**_texto_**`
- Ejemplo: ***negrita y cursiva***

### Listas

**Listas desordenadas**: Se utiliza guion `-`, asterisco `*` o suma `+` seguido de un espacio
````markdown
- Elemento 1
- Elemento 2
- Elemento 3
````

**Listas ordenadas**: Se utilizan números seguidos de punto y espacio
````markdown
1. Hacer el repositorio
2. Clonar el repositorio al local
3. Empezar a escribir en Visual Studio Code
````

### Tablas

Se crean usando barras verticales `|` y guiones `-`:
````markdown
| Nombre   | Edad | Ciudad     |
|----------|------|------------|
| Ana      | 23   | Madrid     |
| Luis     | 31   | Barcelona  |
| Carmen   | 27   | Valencia   |
````

Resultado:

| Nombre   | Edad | Ciudad     |
|----------|------|------------|
| Ana      | 23   | Madrid     |
| Luis     | 31   | Barcelona  |
| Carmen   | 27   | Valencia   |

---
<div id='id4' />

## HTML

HTML es el lenguaje de marcas estándar para crear páginas web. El lenguaje más importante de internet dado que sin HTML no se vería nada en el navegador.

### Estructura básica
````html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primera página</title>
</head>
<body>
    <!-- Aquí va el contenido visible de la página -->
</body>
</html>
````

### Etiquetas de texto

**Encabezados**: Van desde `<h1>` (más grande) hasta `<h6>` (más pequeño)
````html
<h1>Título principal</h1>
<h2>Subtítulo</h2>
````

**Párrafos**: `<p>Texto del párrafo</p>`

**Línea horizontal**: `<hr>`

**Énfasis**:
- Cursiva: `<em>texto en cursiva</em>`
- Negrita: `<strong>texto en negrita</strong>`

### Etiquetas de formulario

- **`<form>`**: Contenedor principal del formulario
````html
  <form action="/enviar" method="post">
      <!-- Campos del formulario -->
  </form>
````

- **`<input>`**: Crea campos de entrada interactivos
````html
  <input type="text" name="nombre" placeholder="Tu nombre">
  <input type="email" name="correo">
  <input type="password" name="contraseña">
````

- **`<select>` y `<option>`**: Menú desplegable
````html
  <select name="ciudad">
      <option value="madrid">Madrid</option>
      <option value="barcelona">Barcelona</option>
  </select>
````

- **`<button>`**: Botón interactivo
````html
  <button type="submit">Enviar</button>
````

### Etiquetas de tabla
````html
<table>
    <thead>
        <tr>
            <th>Nombre</th>
            <th>Edad</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ana</td>
            <td>23</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="2">Total: 1 persona</td>
        </tr>
    </tfoot>
</table>
````

**Descripción de etiquetas**:
- `<table>`: Define la tabla
- `<thead>`: Encabezado de la tabla
- `<tbody>`: Cuerpo de la tabla
- `<tfoot>`: Pie de la tabla
- `<tr>`: Fila de la tabla
- `<th>`: Celda de encabezado
- `<td>`: Celda de datos

---
<div id='id5' />

## Introducción a CSS

CSS (Cascading Style Sheets) es el lenguaje que se utiliza para dar estilo y diseño a las páginas web creadas con HTML. Mientras HTML define la estructura y el contenido, CSS controla cómo se ve ese contenido.

### Características principales de CSS

- **Separación de contenido y presentación**: Permite mantener el HTML limpio enfocado en la estructura
- **Reutilización de estilos**: Esto consigue que un mismo estilo pueda aplicarse a múltiples elementos
- **Control preciso del diseño**: Ofrece propiedades para controlar colores, tipografías, espaciados, posicionamiento y mucho más
- **Diseño responsive**: Permite adaptar la web a diferentes tamaños de pantalla mediante media queries
- **Cascada y especificidad**: Los estilos se aplican según reglas de prioridad y herencia

### Formas de aplicar CSS

**CSS en línea (inline)** - Este CSS aparece justo en la etiqueta del HTML que se quiere cambiar:
```html
Texto azul
```

**CSS interno** - Este CSS aparece en el head con la etiqueta `<style>`, es parecido al CSS externo pero este se encuentra en el HTML:
```html
        p {
            color: blue;
            font-size: 16px;
        }
```

**CSS externo (archivo separado)** - Se crea un .css a parte y se enlaza desde el HTML:
```html
<head>
    <link rel="stylesheet" href="estilos.css">
</head>

```
### Box Model

Todos los elementos HTML son cajas rectangulares compuestas por:

- **Content**: El contenido del elemento (texto, imagen, etc.)
- **Padding**: Espacio interior entre el contenido y el borde
- **Border**: El borde de la caja
- **Margin**: Espacio exterior que separa la caja de otros elementos

```css
div {
    width: 200px;
    padding: 10px;
    border: 2px solid black;
    margin: 20px;
    box-sizing: border-box; /* Incluye padding y border en el ancho total */
}
```