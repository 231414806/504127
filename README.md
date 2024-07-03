# Python Funtions 
Función Python para crear artículo HTML Usted Arma la siguiente función en python: Crea un artículo con el texto escrito dentro de la etiqueta `head` en el documento de tipo HTML.

1. **Usando Flask:**
   Flask es un popular framework de desarrollo web en Python. Puedes generar contenido HTML de forma dinámica utilizando Flask. Aquí tienes un ejemplo simple de cómo crear una página HTML con Flask:

   ```python
   from flask import Flask, render_template

   app = Flask(__name__)

   @app.route('/')
   def index():
       # Contenido para la etiqueta <head>
       head_content = "<title>Mi Página</title>"

       # Renderiza el archivo HTML con el contenido
       return render_template('template.html', head_content=head_content)

   if __name__ == '__main__':
       app.run()
   ```

   En este ejemplo, debes crear un archivo `template.html` en la carpeta `templates` con la estructura HTML deseada. Luego, Flask reemplazará la variable `head_content` con el contenido que quieras incluir dentro de la etiqueta `<head>`.

2. **Incorporando Python en un archivo HTML:**
   Puedes incluir código Python directamente en un archivo HTML utilizando las etiquetas `<script>` y `<style>`. Aquí está un ejemplo básico:

   ```html
   <!DOCTYPE html>
   <html>
   <head>
       <title>Mi Página</title>
       <script>
           // Código Python aquí
           console.log('¡Hola desde Python!');
       </script>
   </head>
   <body>
       <!-- Resto del contenido -->
   </body>
   </html>
   ```

   En este caso, el código Python se ejecutará en el navegador del cliente cuando cargue la página.

 ```Py
from prettytable import PrettyTable
```

# Crear una tabla con dos columnas

```Py
tabla = PrettyTable()
tabla.field_names = ["Pokémon", "Tipo"]
tabla.add_row(["Wartortle", "Agua"])
tabla.add_row(["Charizard", "Fuego/Volador"])
tabla.add_row(["Pikachu", "Eléctrico"])
```

# Imprimir la tabla

```Py
print(tabla)
```
