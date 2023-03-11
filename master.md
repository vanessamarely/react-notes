---
description: >-
  Esta página esta creada con el objetivo de compartir algunas notas sobre
  REACT, que te puedan ayudar en tus proyectos personales o laborales.
---

# ⚛ React

React es una librería que nos ayuda a crear de una forma sencilla SPA (Single Page Aplication) o como dice en su página oficial, nos permite crear interfaces de usuario.

React no es un framework, en conjunto con otras librerías, se convierte en una gran solución o una potente herramienta parecida a un framework, para ayudarnos a crear nuestras aplicaciones de una forma rápida.

Existen una gran cantidad de conceptos que envuelven A React que es importante conocer y espero poderlos abordar poco a poco en esta guía.

Para trabajar exitosamente con React es necesario saber Javascript. De los conceptos más importantes de Javascript es necesario conocer:

* Variables y tipos de datos
* Objetos y Arrays
* Funciones y Classes
* Estructuras de datos: condicionales y ciclos (loops)

Otros conceptos útiles son:

* Spread operator, arrow functions, ente otros provenientes desde el ES6

En React existen diferentes conceptos como:&#x20;

* Componentes
* JSX
* Stateful/ Stalteess component
* Hooks
* entre otros

## DOM (Modelo de objetos del Documento)

El DOM es el árbol de objetos, de los elementos que se encuentran en el documento HTML.

Tengo un articulo en [`medium`](https://vanessamarely.medium.com/crp-critical-render-path-o-ruta-de-acceso-de-representaci%C3%B3n-cr%C3%ADtica-1f2ca78d2645) `` o en [dev.to](https://dev.to/vanessamarely/crp-critical-render-path-o-ruta-de-acceso-de-representacion-critica-31eh), donde puedes ampliar la información sobre el critical render path y conocer un poco más sobre el DOM y como se renderiza en los navegadores.



## Virtual DOM

Es la copia del DOM en memoria, que analiza los cambios que se realizan en el DOM y los compara, para proceder solo a ejecutar o renderizar esos elementos en el DOM, sin tener que modificar todo el árbol.

## Componentes

Un componente podríamos mirarlo como una pequeña parte de nuestra aplicación. Visualmente podemos decir que un componente puede ser una lista, un elemento de la lista, o la página donde incluiremos otros elementos.&#x20;

Desde una parte lógica, podemos decir que un componente es una función de Javascript, donde podemos tener parámetros de entrada, algunos de salida, llamar a funciones y retornar elementos.

Un componente de React será una función o una clase que puede retornar un elemento HTML o JSX.



## **Interpolación**

es decirle a un elemento que va a incluir otro que puede ser de otra naturaleza. Por ejemplo para mostrar una variable en un atributo o en el JSX entre llaves, asignaremos el nombre.

```html
<img src={image} alt={name} />
```



## JSX

Es una extension de la sintaxis de javascript, que produce elementos de React.

JSX permite hacer una separación de intereses, no tienes que crear un archivo de HTML aparte para manejar y uno de javascript. Para evitarte esa preocupación se integran el lenguaje de marcado con la lógica de javascript.&#x20;

No es obligatorio usar JSX, para crear los componentes de React, pero visualmente es mucho mas sencillo de manejar.



## Stateful & Stateless&#x20;



**Stateless**, es llamado sin estado, son componentes de presentación o componentes que solo van a mostrar información. Son llamados componentes tontos

**Stateful** son componentes con estado, en ellos va a ocurrir una mayor lógica, pueden ser componentes donde se van a hacer llamados al server o peticiones. Estos componentes llaman a los componentes Stateless. Son llamados también componentes smart.

## Props

Los props son propiedades de React. estas propiedades se declaran en la etiqueta de componente como atributos y en la función del componente se reciben como parámetros, o propiedades que se necesitan compartir entre padres e hijos.



## Manejo de Eventos&#x20;



Manejar eventos es muy similar a como se realizaría en el DOM y en las etiquetas HTML. los eventos se debe usar en camelCase (palabras compuestas), en lugar de minúsculas. Ademas se debe pasar una función en el evento usando la interpolación.

{% hint style="info" %}
**camelCase**, con palabras compuestas de una o más palabras donde se puede iniciar en minúscula y las siguientes palabras deben comenzar con mayúscula inicial. Por ejemplo:

**variableCompuesta**
{% endhint %}

<pre class="language-javascript"><code class="lang-javascript">&#x3C;button onClick={handleClick>
<strong>    Click
</strong>&#x3C;/button>
</code></pre>

```javascript
const handleClick = () => console.log('click me');
```

## Ciclo de Vida de los componentes

Los componentes de React, anteriormente ejecutaban varias clases en su ciclo de vida. Se puede decir que lo mas básico en el ciclo de vida de un componente es que este se Monte, se Actualice y Desmonte.





## Hooks



Son funciones de javascript, que nos permiten crear y acceder al estado de un componente y controlar su ciclo de vida.

### Hook de estado: useState



Nos permite añadirle un estado al componente y modificar ese estado.

```javascript
const [showMessage, setShowMessage] = useState(false);
```

### Hook de efecto: useEffect



Estas funciones nos permiten reemplazar las clases que se usaban para ejecutar el ciclo de vida de React. Tambien en este Hook podemos realizar peticiones a apis.

```javascript
useEffect(() => {
   console.log('se ha ejecutado el hook');
 }, [name]);
```

