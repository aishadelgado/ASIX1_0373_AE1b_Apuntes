# ASIX1_0373_AE1b_Apuntes

## Índice
1. **[GitHub](#id1)**
2. **[Git](#id2)**
3. **[Markdown](#id3)**
4. **HTML**

<div id='id1' />

### GitHub
---

<p align="center">
	<img src="img/github-logo.jpg" alt="GitHub logo" style="max-width:360px; width:60%; height:auto;">
</p>

GitHub es una plataforma en la nube que se utiliza para alojar proyectos de software, permitiendo a los desarrolladores colaborar, compartir y gestionar cambios en el código de forma remota.

Nosotros lo que hicimos en clase fue crearnos una cuenta, los que veníamos de SMX ya la teníamos creada, y una vez lista pues arriba a la izquierda, donde aparecen una lista de repositorios, creamos cada uno de los repositorios que iremos haciendo y utilizando por cada trabajo que hagamos.

A la hora de crear un repositorio nos pedirá varias cosas, siendo las peticiones las siguientes:
- Nombre del repositorio
- Breve descripción
- Si será un repositorio público o privado
- Si se le quiere añadir un ReadMe o no (en este punto lo mejor siempre es añadirle uno, porque sino luego hay que hacer más cosas para poder trabajar en el repositorio)

Una vez todo escrito y seleccionado, solamente quedará darle a crear el repositorio, así ya nos aparecerá el repositorio en nuestra cuenta.

<div id='id2' />

### Git
---

Git se utiliza principalmente para gestionar el historial de cambios en archivos de código fuente, permitiendo que múltiples desarrolladores colaboren en un proyecto de manera simultánea.
En nuestro caso lo utilizaremos para poder hacer todos los commits que vayamos haciendo en el Visual Studio Code.
Primero que nada se tendrá que instalar el Git para poder hacerlo funcionar en el cmd.

Una vez instalado, los comandos que se tendrán que utilizar serán los siguientes:
- _git clone_: Este comando, seguido de la url de nuestro repositorio, creará una carpeta clonada del repositorio.
- _git init_: Este comando nos servirá para inicializar la carpeta que se vaya a utilizar en el momento, así los próximos comandos de git que se utilicen irán directamente a esa carpeta.
- _git add_: Esto nos servirá para que, después de cambiar, añadir o eliminar cosas en nuestro visual, este comando lo encuentre. Para que haga todo se deberá utilizar un punto al final ".".
- _git commit -m_: Este comando nos servirá para hacer los commits que irán a parar a nuestro repositorio. Para escribirle un título al commit se tendrá que escribir entre comillas.
- _git push origin main_: Este es el comando que hace que los commits terminen en el github.

Hecho todo esto, ya tendrás el commit enviado de tu local al GitHub.

<div id='id3' />

### Markdown
---

Markdown es un lenguaje de marcas ligero que permite crear documentos con formato de manera sencilla y legible. Se usa mucho en archivos README, documentación y foros.

Ahora haré una explicación básica con sus respectivos ejemplos de etiquetas comunes:
- **Encabezados**

Las almohadillas (#) se utilizan al principio de una línea, seguido de un espacio (así funcionará), para poder hacer encabezados, como ya he hecho con el índice, markdown, etc.
Un ejemplo de esto sería: `# Hola mundo`, esto lo que haría sería hacer en un encabezado h1 ese escrito.
Se pueden utilizar hasta 6 almohadillas a la vez, si se utiliza solo una será más grande y si se utilizan las 6 será cada vez más pequeño.

- **Negrita y cursiva**

Para la negrita y cursiva se utilizan los asteriscos o guiones bajos, dependiendo de lo que se quiera hacer se utilizarán más o menos.
Para la **negrita** se puede hacer con dos asteríscos `**negrita**` o con dos guiones bajos `__negrita__`
Por otro lado, para la _cursiva_ se utiliza o un asterísco `*cursiva*` o un guion bajo `_cursiva_`
Si se quieren utilizar las dos a la vez, hay dos formas distintas, la primera sería utilizar tres asteríscos `***negrita y cursiva***`. La otra forma sería utilizando los asteriscos y guiones, justo así `**_negrita y cursiva_**`.

- **Listas desordenadas**

Para las listas desordenadas se utilizará el guion al inicio, seguido de un espacio para separar la marca del texto. No pondré ejemplo pero es lo que estoy haciendo para separar cada punto del markdown.

- **Listas ordenadas**

Para las listas ordenadas se utilizarán los números de forma autonumérica, es decir, si se empieza con un 1. el siguiente no puede ser un 3.
Ejemplo de una lista ordenada:
1. Hacer el repositorio
2. Clonar el repositorio al local
3. Empezar a escribir en el Visual Studio Code

- **Tablas**

Las tablas se crean usando | y -:

| Nombre   | Edad | Ciudad     |
|----------|------|------------|
| Ana      | 23   | Madrid     |
| Luis     | 31   | Barcelona  |
| Carmen   | 27   | Valencia   |

`| Nombre   | Edad | Ciudad     |`
`|----------|------|------------|`
`| Ana      | 23   | Madrid     |`
`| Luis     | 31   | Barcelona  |`
`| Carmen   | 27   | Valencia   |`

