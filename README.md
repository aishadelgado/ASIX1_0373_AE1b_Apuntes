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

Markdown es un lenguaje de marcas ligero que se utiliza para dar formato a texto de manera sencilla y rápida, sin necesidad de usar etiquetas complejas como en HTML. Fue creado para que las personas pudieran escribir contenido con formato (títulos, listas, enlaces, código, etc.) usando solo texto plano, de una forma fácil de leer y de escribir.

A diferencia de HTML, Markdown no está pensado para navegadores. Su sintaxis es simple e intuitiva, lo que permite que el texto sea comprensible incluso antes de ser convertido o renderizado. Por ejemplo, un archivo Markdown puede leerse sin problemas en cualquier editor de texto.

Markdown no reemplaza a HTML, sino que lo simplifica. De hecho, muchos sistemas convierten automáticamente Markdown en HTML para mostrarlo en la web.

### Encabezados

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

HTML (HyperText Markup Language) es el lenguaje estándar utilizado para crear y estructurar páginas web. Es la base de cualquier sitio web que se ve en Internet. Cada vez que se entra a una página, el navegador interpreta un documento HTML para mostrar textos, imágenes, enlaces, botones y otros elementos visuales.

HTML no es un lenguaje de programación, ya que no ejecuta lógica ni cálculos. En lugar de eso, es un lenguaje de marcas, lo que significa que utiliza etiquetas para indicar al navegador qué tipo de contenido es cada parte del documento y cómo debe organizarse dentro de la página.

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

**Encabezados**: Van desde `<h1>` que es el más grande hasta `<h6>` que es el más pequeño
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

En los orígenes de la web, HTML era muy sencillo y fácil de aprender y no era capaz de representar recursos gráficos para añadir a la información textual. Eso fue cambiando a medida que el número de sitios web fueron creciendo y con ellos la cantidad de etiquetas que HTML se necesitaba para construir sitios cada vez más atractivos. Se tenían que incluir nuevas etiquetas destinadas a conseguir efectos visuales.

CSS (Cascading Style Sheets) es el lenguaje que se utiliza para dar estilo y diseño a las páginas web creadas con HTML. Mientras HTML define la estructura y el contenido, CSS controla cómo se ve ese contenido.

### Ventajas e inconvenientes

Las ventajas de usar hojas de estilo son:

- Posibilidad de mantener el código más fácilmente
- A nivel de diseño, CSS es más potente que las etiquetas de diseño de (X)HTML
- CSS es un lenguaje sencillo
- Se pueden definir diferentes hojas de estilo para un solo documento (X)HTML, por ejemplo, un estilo para la página web cuando se visita desde un ordenador y otra para cuando queramos imprimirla
- Se puede reutilizar desde diferentes documentos (X)HTML

El único y mayor inconveniente es que no todos los navegadores se comportan de la misma forma ante una hoja de estilo dado que algunos no cumplen con los estándares establecidos. Así, obligan al programador a crear diferentes hojas de estilo.

### Características principales de CSS

- **Separación de contenido y presentación**: Permite mantener el HTML limpio enfocado en la estructura
- **Reutilización de estilos**: Esto consigue que un mismo estilo pueda aplicarse a múltiples elementos
- **Control preciso del diseño**: Ofrece propiedades para controlar colores, tipografías, espaciados, posicionamiento y mucho más
- **Diseño responsive**: Permite adaptar la web a diferentes tamaños de pantalla mediante media queries
- **Cascada y especificidad**: Los estilos se aplican según reglas de prioridad y herencia

### Formas de aplicar CSS

**CSS en línea (inline)** - Este CSS aparece justo en la etiqueta del HTML que se quiere cambiar:
```html
	<p style="color: blue; font-size: 16px;">Texto azul</p>
```

**CSS interno** - Este CSS aparece en el head con la etiqueta `<style>`, es parecido al CSS externo pero este se encuentra en el HTML:
```html
        <head>
			<style>
				p {
					color: blue;
					font-size: 16px;
				}
			</style>
		</head>
```

**CSS externo (archivo separado)** - Se crea un .css a parte y se enlaza desde el HTML:
```html
<head>
    <link rel="stylesheet" href="estilos.css">
</head>

```

### Prioridad

La **prioridad** (también llamada **especificidad**) determina qué estilos se aplican cuando hay reglas CSS conflictivas que afectan al mismo elemento. Entender la prioridad es fundamental para escribir CSS mantenible y predecible.

#### La Cascada

La cascada determina qué regla se aplica cuando múltiples reglas coinciden con el mismo elemento, siguiendo este orden de prioridad de menor a mayor:

1. Estilos del navegador
2. Estilos del usuario
3. Estilos del autor
4. Estilos del autor con `!important`
5. Estilos del usuario con `!important`

#### Especificidad

La especificidad es un sistema de puntuación que determina qué selector tiene más peso cuando hay conflicto. Se calcula como una combinación de cuatro valores: inline, IDs, Classes, Elements.

##### Reglas de prioridad

- **De mayor a menor prioridad:**

1. **Estilos inline:** Son los estilos escritos directamente en el HTML, dentro del atributo `style=""`. Tienen la mayor prioridad porque están aplicados directamente al elemento.
2. **IDs:** Se aplican a los elementos con un id específico (`#identificador`). Un id debe ser único en la página ya que sino dará errores o los estilos no aparecerán como el usuario desea
3. **Classes, atributos y pseudo-clases:** (`.clase`, `[type="text"]`, `:hover`). Se usan mucho porque son reutilizables.
4. **Elementos y pseudo-elementos** (`div`, `p`, `::before`). Son los selectores más generales.

#### Regla de desempate: Orden en cascada

En CSS, a veces dos o más reglas apuntan al mismo elemento y tienen exactamente la misma especificidad, es decir, pesan lo mismo.
Cuando eso ocurre, CSS necesita una forma de decidir cuál aplicar.

La regla que gana es la que aparece más tarde en el código.
Un ejemplo:

```css
.texto {
    color: blue;
}

.texto {
    color: red;    /* ← GANA porque está después */
}
```

#### Herencia

La herencia en CSS es un mecanismo que permite que algunas propiedades de estilo aplicadas a un elemento padre se transmitan automáticamente a sus elementos hijos, sin necesidad de volver a escribir esas reglas.

CSS funciona como un árbol de elementos, donde cada elemento puede tener hijos. Cuando una propiedad es heredable, el navegador copia su valor del padre al hijo.

```css
body {
    color: blue;
    font-family: Arial;
}

/* Todos los elementos dentro de body heredarán estos estilos */
```