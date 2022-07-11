# Guide

### GIT
1. Instalar git en windows
https://git-scm.com/download/win
Practicar, creando un folder y archivos
ejecutar luego los siguientes comandos:

2. Crear una carpeta para proyectos
```bash
mkdir projects
```
3. Crear archivo .html de ejemplo, luego agregar contenido
```bash
touch index.html
```
4. Configurar git en local
```bash
git config --global user.name "Your name"
git config --global user.email "Your email"
```
5. Consultar estado de los ficheros, si se ha creado, modificado o eliminado algún fichero
```bash
git status -s
```
4. Para agregar todos los cambios realizados
```bash
git add .
```
5. Confirmar cambios con un mensaje
```bash
git commit -m "Mensaje de commit"
```
6. Confirmar cambios sin un mensaje y sobreescribiendo el commit anterior
```bash
git commit --amend
```
7. Subir cambios a un repositorio
```bash
git push origin master
```
8. Ver ramas creadas en local
```bash
git branch
```
9. Crear una nueva rama
```bash
git checkout -b nuevo-nombre-de-branch
git switch -c nuevo-nombre-de-branch
```
10. Ir hacia otra rama existente
```bash
git checkout otra-branch
git switch otra-branch
```
11. Clonar un repositorio
```bash
git clone nombre-del-repositorio
```
12. Unificar últimos 3 commits en 1 solo. Se pone 's' o 'squash' a las ramas que se unifican excepto la primera
```bash
git rebase -i HEAD~3

pick 910dfc6 mensaje-commit-1
squash 3955d77 mensaje-commit-2
squash c009b49 mensaje-commit-3
```

```bash
Commands:
# p, pick <commit> = use commit
# r, reword <commit> = use commit, but edit the commit message
# e, edit <commit> = use commit, but stop for amending
# s, squash <commit> = use commit, but meld into previous commit
# f, fixup [-C | -c] <commit> = like "squash" but keep only the previous
#                    commit's log message, unless -C is used, in which case
#                    keep only this commit's message; -c is same as -C but
#                    opens the editor
# x, exec <command> = run command (the rest of the line) using shell
# b, break = stop here (continue rebase later with 'git rebase --continue')
# d, drop <commit> = remove commit
# l, label <label> = label current HEAD with a name
# t, reset <label> = reset HEAD to a label
# m, merge [-C <commit> | -c <commit>] <label> [# <oneline>]
# .       create a merge commit using the original merge commit's
# .       message (or the oneline, if no original merge commit was
# .       specified); use -c <commit> to reword the commit message
#
# These lines can be re-ordered; they are executed from top to bottom.
```
13. Ver log de commits
```bash
git log --graph --oneline --decorate --all
```
### HTML
Para practicar maquetación con HTML, CSS y javascript. Se podría recurrir a la página [frontendmentor.io](https://www.frontendmentor.io), como alternativa, gracias los diseños que proporcionan.Aquí listaré algunas etiquetas que se pueden usar:
1. Indica que el HTML es versión 5
```html
<!DOCTYPE html>
```
2. Indica que el HTML es lenguaje Inglés
```html
<html lang="en">
```
3. Meta para formato utf-8
```html
<meta charset="utf-8">
```
4. Meta para sitio web responsive
```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```
5. Ejemplo de meta tags Opengraph de Facebook para SEO
```html
<meta property="og:title" content="Titulo del sitio">
<meta property="og:description" content="Descripción del sitio">
<meta property="og:image" content="URL de la imagen">
<meta property="og:url" content="URL del sitio">
```
6. Agregar estilos en línea: Mala práctica
```html
<style>
  body {
    background-color: #f0f0f0;
  }
</style>
```
7. Agregar estilos en archivo: Forma tradicional
```html
<link rel="stylesheet" href="css/style.css">
```
8. Agregar javascript en línea: Mala práctica
```html
<script>
  function myFunction() {
    console.log("Hola mundo");
  }
  myfunction();
</script>
```
9. Agregar javascript en archivo: Forma tradicional
```html
<script src="js/script.js"></script>
```
10. Agregar javasript en archivo: Soporte de ES6 modules
```html
<script src="js/script.js" type="module"></script>
```
11. Estructura simple de HTML, head, body
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <h1>Hola mundo</h1>
</body>
</html>
```
12. Etiquetas para títulos, descendente por predominancia. No debería agregarse uno de menos jerarquía arriba de uno con más jerarquía.
```html
<h1>Título Principal</h1>
<h2>Título</h2>
<h3>Título</h3>
<h4>Título</h4>
<h5>Título</h5>
<h6>Título</h6>
```
13. Etiqueta para párrafos
```html
<p>Este es un párrafo</p>
```
14. Etiqueta para palabra o palabras más resaltantes
```html
<strong>Esta es una palabra más resaltada</strong>
```
15. Etiqueta para hipervíncular otra página
```html
<a href="https://marioroca.dev" alt="portfolio">Portfolio</a>
```
16. Etiqueta para contener imágenes
```html
<figure>
  <img src="images/image.jpg" alt="image" />
</figure>
```
17. Etiqueta para bloques y secciones
```html
<div></div>
<section></section>
```
18. Etiquetas para listas ordenadas
```html
<ol>
  <li>Elemento 1</li>
  <li>Elemento 2</li>
  <li>Elemento 3</li>
</ol>
```
19. Etiquetas para listas desordenadas
```html
<ul>
  <li>Elemento 1</li>
  <li>Elemento 2</li>
  <li>Elemento 3</li>
</ul>
```
20. Etiqueta para tarjetas o artículos de texto que contengan título, imagen, párrafo como mínimo.
```html
<article>
  <h2>Títular</h2>
  <img src="images/banner.jpg" alt="Banner" />
  <p>Descripción o contenido del artículo</p>
  <a href="/destacada" title="Banner">Ver más</a>
</article>
```
21. Etiquetas cuyo display es inline
```html
<span>Este es un texto menor</span>
<strong>Esta es una texto más resaltante</strong>
<i>texto en cursiva<i>
<b>texto en negrita</b>
```
22. Etiquetas para acordeones nativos
```html
<details>
  <summary>Detalle de algo</summary>
  Detalle de ese algo, luego de expandirlo
</details>
<details open>
<summary>Item 2</summary>
  Alguna descripción luego de expandirlo
</details>
```
23. Etiquetas para fechas
```html
<time datetime="2022-01-01">01/01/2022</time>
```
24. Etiquetas para hacer un selector autocomplete
```html
<label for="car">Selecciona Car:</label>
<input list="cars" id="car" name="cars" placeholder="Seleccionar car.." />
<datalist id="cars">
  <option value="BMW">
  <option value="Tesla">
  <option value="Toyota">
  <option value="Volkswaggon">
  <option value="Mazda">
</datalist>
```
25. Etiquetas para formularios: input tipo texto
```html
<label for="name">Nombre:</label>
<input type="text" id="name" name="name" placeholder="Nombre" />
```
26. Etiquetas para formularios: input tipo email
```html
<label for="email">Email:</label>
<input type="email" id="email" name="email" placeholder="Email" />
```
27. Etiquetas para formularios: input tipo password
```html
<label for="password">Contraseña:</label>
<input type="password" id="password" name="password" placeholder="Contraseña" />
```
28. Etiquetas para formularios: input tipo tel, para teléfonos o tarjeta de crédito
```html
<label for="tel">Teléfono:</label>
<input type="tel" id="tel" name="tel" placeholder="Teléfono" />
```
29. Etiquetas para formularios: input tipo date, para fechas con datapicker
```html
<label for="date">Fecha:</label>
<input type="date" id="date" name="date" placeholder="Fecha" />
```
30. Etiquetas para formularios: input tipo number, para números
```html
<label for="number">Número:</label>
<input type="number" id="number" name="number" placeholder="Número" />
```
31. Etiquetas para formularios: input tipo range, para números con un rango
```html
<label for="range">Rango:</label>
<input type="range" id="range" name="range" placeholder="Rango" />
```
32. Etiquetas para formularios: input tipo checkbox, para checkbox
```html
<label for="checkbox">Checkbox:</label>
<input type="checkbox" id="checkbox" name="checkbox" />
```
33. Etiquetas para formularios: input tipo radio, para radio
```html
<label for="radio">Radio:</label>
<input type="radio" id="radio" name="radio" />
```
34. Etiquetas para formularios: input tipo submit, para botón submit
```html
<input type="submit" id="submit" name="submit" value="Enviar" />
```
35. Etiquetas para formularios: input tipo reset, para botón reset
```html
<input type="reset" id="reset" name="reset" value="Limpiar" />
```
36. Etiquetas para formularios: input tipo file, para seleccionar archivos
```html
<label for="file">Archivo:</label>
<input type="file" id="file" name="file" />
```
37. Etiquetas para formularios: input tipo hidden, para ocultar datos
```html
<input type="hidden" id="hidden" name="hidden" value="hidden" />
```
38. Etiquetas para formularios: input tipo search, para hacer búsquedas
```html
<label for="search">Buscar:</label>
<input type="search" id="search" name="search" placeholder="Buscar" />
```
39. Etiquetas para formularios: input tipo color, para seleccionar color
```html
<label for="color">Color:</label>
<input type="color" id="color" name="color" />
```
40. Etiquetas para formularios: textarea
```html
<label for="textarea">Textarea:</label>
<textarea id="textarea" name="textarea" placeholder="Textarea"></textarea>
```
41. Etiqueta de formulario y ejemplo de formulario básico
```html
<form action="/my-handling-form-page" method="post">
  <ul>
    <li>
      <label for="name">Nombre:</label>
      <input type="text" id="name" name="user_name">
    </li>
    <li>
      <label for="mail">Correo electrónico:</label>
      <input type="email" id="mail" name="user_mail">
    </li>
    <li>
      <label for="msg">Mensaje:</label>
      <textarea id="msg" name="user_message"></textarea>
    </li>
  </ul>
</form>
```

## CSS
Mientras más diseños se hagan, más se aprenderá para qué es puede servir cada instrucción de CSS

##### Selectores en CSS
1. Para seleccionar todo en el html, etiquetas y pseudoelementos
```css
* {
  margin: 0;
  padding: 0;
}
```
2. Para seleccionar una clase
```css
.nombre-de-clase {
  color: red;
}
```
3. Para seleccionar por un id
```css
#nombre-de-id {
  color: blue;
}
```
4. Para seleccionar por etiqueta
```css
p {
  color: green;
}
```
4. Para seleccionar por un atributo
```css
[atributo="valor"] {
  color: green;
}
```
5. Para seleccionar elemento directo
```css
div > p {
 color: orange;
}
```
6. Para seleccionar elemento que contiene el nombre de alguna clase
```html
  <article class="nombre-clase-1 nombre-clase-2 nombre-clase-3"></article>
```
```css
article[class~="nombre-clase-1"]{
  color: orange;
}
```
