# Bootstrap 4

Existen 2 formas para utilizar Bootstrap:

**CDN**

Referencia a los css y a 3 archivos javascript que están en la web.

1. Referencia a JQuery
2. Referencia a Popper.JS: Esta herramienta nos sirve para crear los popUps (esos mensajes flotantes que se muestran al posicionar el cursor en un lugar predeterminado)
3. JS de bootstrap.
4. CSS de Bootstrap

Por otro lado, noten que cada referencia contiene un .min dentro de sus nombres (por ejemplo; bootstrap.min.css, …jquery-3.3.1.slim.min.js, etc) que no es más que la versión minificada(sin espacios) de cada archivo de código.


**Descargando los archivos comprimidos**

Otra de las opciones es descargando todos los archivos que componen Bootstrap y añadiendolos a tu proyecto. Esta opción es interesante ya que te permite trabajar sin conexión a internet, cosa que no puedes hacer con la opción anterior.

## Hola mundo

[Introducción a Bootstrap](https://getbootstrap.com/docs/4.3/getting-started/introduction/)

[Layout](https://getbootstrap.com/docs/4.3/layout/overview/)

## Template de inicio

[Template](https://getbootstrap.com/docs/4.3/getting-started/introduction/#starter-template)


### Etiquetas importantes

**HTML5**

```HTML
<!doctype html>
<html lang="es">
  ...
</html>
```


**Meta tag viewport**

Bootstrap se desarrolla primero para dispositivos móviles, una estrategia en la que primero optimizamos el código para dispositivos móviles y luego ampliamos los componentes según sea necesario mediante consultas de medios CSS. Para garantizar una representación adecuada y un zoom táctil para todos los dispositivos, agregue la meta tag siguiente:

```html
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

```


## Grid, grilla o cuadrícula

### Container

Componente más básico y es requerido si queremos usar la grid de Bootstrap

Lo agregamos con un div y la siguiente clase

```html

<div class="container">
  ...
</div>

```

Vemos que tiene un ancho fijo que permanece hasta que su resolución o ancho de la pantalla disminuye y ocupa todo el ancho de la pantalla.

Ahora probemos con la clase `container-fluid`
Veremos que ocupa todo el ancho de la pantalla.


### Row

Para crear columnas, que es lo que queremos, siempre necesitamos crear con anterioridad *filas*

Lo haremos de la siguiente forma:

```html
<div class="row">

</div>

```

### Columnas

```html

  <div class="col">
    1
  </div>
  <div class="col">
    2
  </div>
  <div class="col">
    3
  </div>

```

La clase `col` me agrega columnas que tienen cierto espacio. Al no especificar ningún tamaño de las columnas. Estas se van a repartir el ancho disponible equitativamente.

```html
<div class="row">
  <div class="col">
    1
  </div>
  <div class="col">
    2
  </div>
  <div class="row">
    <div class="col">
      1
    </div>
    <div class="col">
      2
    </div>
    <div class="col">
      3
    </div>
  </div>
</div>
