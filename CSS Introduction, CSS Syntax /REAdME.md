1. CSS Externo
Se utiliza para definir el estilo de todo un sitio web mediante un único archivo con extensión .css
. Para implementarlo, se debe incluir una referencia al archivo externo usando la etiqueta <link> dentro de la sección <head> de la página HTML
EJEMPLO:
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>

2. CSS Interno
Esta modalidad se emplea cuando una sola página HTML requiere un estilo único y específico
Las reglas se definen dentro del elemento <style>, el cual debe ubicarse dentro de la sección <head> del documento
Ejemplo:
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
} 
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
3. CSS en línea
El estilo en línea se usa para aplicar una regla exclusiva a un único elemento HTML
Se realiza agregando el atributo style directamente en la etiqueta del elemento correspondiente

Ejemplo:
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>

4. Orden en cascada y múltiples hojas de estilo
Cuando un elemento tiene más de un estilo definido, el navegador sigue un orden de prioridad para decidir cuál aplicar
Si se definen propiedades en diferentes hojas de estilo para el mismo selector, prevalecerá la última que el navegador lea.El orden general de prioridad (de mayor a menor) es el siguiente:
Estilo en línea (máxima prioridad)
Hojas de estilo externas e internas (según el orden en que aparezcan en el encabezado)
Configuración predeterminada del navegador
EJEMPLO:
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
body {background-color: linen;}
</style>
</head>
<body style="background-color: lavender">

<h1>Multiple Styles Will Cascade into One</h1>
<p>Here, the background color of the page is set with inline CSS, and also with an internal CSS, and also with an external CSS.</p>
<p>Try experimenting by removing styles to see how the cascading stylesheets work (try removing the inline CSS first, then the internal, then the external).</p>

</body>
</html>


