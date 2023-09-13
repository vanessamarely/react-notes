---
description: Este taller pretende darte el primer acercamiento al uso de React.
---

# 👩💻 Crea tu primera App en React

### 🤔 **¿Qué es React?**

Es una biblioteca o librería de Javascript (**EcmaScript**) para crear interfaces de usuario.

## 🛠️ Herramientas

Para este taller vamos a usar [`Stackblitz`](https://stackblitz.com/), y tu cuenta de [`Github`](https://github.com/) para que te puedas hacer login o 'sign in' en ella, al usar el editor online.



Si aún no tienes tu cuenta de Github y deseas saber como crearla puedes ver la guía en las sección de guías utiles.

{% embed url="https://app.gitbook.com/s/-LVsT1Ma_vwr-w-uljBc/guias-utiles/github" %}

También encontraras en las guías utiles una sección de IDEs, donde te mostrare paso a paso crear un proyecto en stackblitz.



{% embed url="https://app.gitbook.com/s/-LVsT1Ma_vwr-w-uljBc/guias-utiles/ides" %}

## 🌟 Iniciemos a crear nuestra App



Para este taller usaremos el IDE online llamado stackblitz.&#x20;



Así que siguiendo el paso a paso de la guía de IDE. Crearemos nuestro proyecto en React javascript.



<figure><img src="../.gitbook/assets/Screenshot 2023-03-08 at 4.12.21 PM.png" alt=""><figcaption><p>Hela Mundo en stackblitz</p></figcaption></figure>

### 🔍 Explorando el Hola Mundo, generado por stackblitz



En la estructura de carpetas podrás apreciar en los Files, que se ha creado una carpeta public y una carpeta `src`



<figure><img src="../.gitbook/assets/Screenshot 2023-03-08 at 4.32.09 PM.png" alt=""><figcaption><p>Estructura de carpetas</p></figcaption></figure>

Toda aplicación parte de un documento HTML. En la carpeta public al seleccionar el `index.html`, se puede encontrar el contenedor de nuestra aplicación.

{% code lineNumbers="true" %}
```html
// Contenedor de la App

<div id="root"></div>

```
{% endcode %}

<figure><img src="../.gitbook/assets/Screenshot 2023-03-08 at 4.38.17 PM.png" alt=""><figcaption><p>index.html</p></figcaption></figure>



{% hint style="info" %}
Si vamos a los conceptos del HTML. Un documento HTML es compuesto por etiquetas. Entre esas etiquetas existe una muy general llamada div -> `<div></div>`

Las etiquetas tienen atributos que dan características a la etiqueta. En este caso se va a hacer uso del id y se le asigna el valor de root.

Este atributo puede ser usado en el css, como un selector de identificación y usado en javascript, haciendo uso del objeto document o el window.
{% endhint %}



Explorando nuestra carpeta `src`, encontramos tres archivos: **`App.js`**, **`index.js`**, y **`style.css`**

<figure><img src="../.gitbook/assets/Screenshot 2023-03-08 at 4.45.35 PM.png" alt=""><figcaption><p>carpeta src</p></figcaption></figure>

**`App.js`**, es el archivo donde se crea nuestro primer componente de React.

<figure><img src="../.gitbook/assets/Screenshot 2023-03-08 at 4.53.27 PM.png" alt=""><figcaption></figcaption></figure>

En nuestro proyecto como estamos usando un IDE online, este internamente tiene integrado diferentes herramientas, que permiten manejar diferentes paquetes o librerías.&#x20;

Las primeras lineas de javascript son **`imports`**, que nos permiten importar el primero la librería y el segundo nuestra hoja de estilos

{% hint style="info" %}
**import**, es una palabra reservada de javascript o por decirlo de otra forma es un termino que se usa, para importar funciones que han sido exportados desde otro **modulos** (otras funciones).
{% endhint %}

En la linea 4, encontramos una función de javascript declarada con el nombre App, que esta siendo exportada por defecto haciendo uso del **`export`**.

{% hint style="info" %}
**export**, es una palabra reservada o termino para referirse a un modulo que se crea, que exporta funciones, que pueden ser usadas en otros archivos, mediante el **import**.
{% endhint %}

Hablando de **`App`**, es una función o componente. Esta función esta retornando, mediante la palabra reservada return, nuestros elementos HTML. La sintaxis del HTML dentro del javascript es lo que se conoce como JSX.&#x20;

**`index.js`**, es el archivo donde se hace uso del identificador, declarado en el HTML. Y haciendo uso de las funciones de React, se create el elemento contenedor de nuestro componente, para pasarlo al documento, haciendo uso del DOM (Document Object Model).

{% hint style="info" %}
DOM (Document Object Model) o modelo de objetos del documento. El DOM nos permite la manipulación de las etiquetas del documento, por medio de javascript.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 4.25.09 PM.png" alt=""><figcaption></figcaption></figure>

En la primera linea del **`index.js`** se importa la libreria de React y el `StrictMode`.

En la segunda linea se importa el **`react-dom`**, librería necesaria al igual que la primera para trabajar con los elementos del DOM de React.



En la linea 4, se importa el componente `App`, el componente general de nuestra aplicación.

En la linea 6 y 7 se crean dos constantes. La primera es la que obtiene del HTML el identificador. La segunda constante crea un elemento de React, que se encargara de indicarle a React, que crearemos un elemento el cual haciendo uso del identificador, mostrara todo lo que contenga la función render, del elemento root; que serán las lineas del 9 al 14.

Dentro del render, tenemos las etiquetas **`StrictMode`**, cuya función es ejecutar javascript en modo estricto. Esta nos indica que se van a comprobar los elementos que se usen para evitar posibles errores al hacer el código. Y dentro del **`StrictMode`**, tenemos el componente App.

**`style.css`**, es la hoja de estilos de nuestro documento. En ella crearemos todo el formato que deseemos crear a nuestro proyecto de forma general. Como por ejemplo, incluir una fuente, crear variables, etc.

La hoja de estilos contiene por defecto algunos selectores de etiqueta como el **`h1`** y el **`p`**, a los cuales se les esta especificando un tipo de fuente.

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 4.33.41 PM.png" alt=""><figcaption></figcaption></figure>

## 1. Carguemos una fuente de Google Fonts



La pagina de Google fonts, nos trae varias opciones para cambiar la fuente de nuestro proyecto. Para nuestro proyecto vamos a hacer uso de open sans.

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 4.36.24 PM.png" alt=""><figcaption></figcaption></figure>

Para usar una fuente la buscamos, usando el buscador de la pagina.

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 4.38.15 PM.png" alt=""><figcaption></figcaption></figure>

La seleccionamos, y nos abre una pagina con diferentes tipos de la fuente, puedes seleccionar todos los que desees cargar para tu fuente, dando click en la opción que dice Select en azul.

Al seleccionar se mostrara una ventana donde se te indica como puedes usar la fuente.

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 4.40.24 PM.png" alt=""><figcaption></figcaption></figure>



En este caso vamos a seleccionar el `@import`, para insertar nuestra fuente en el archivo `style.css`

Copiamos el contenido dentro de las etiquetas `<style></style>` y lo pegamos al inicio de nuestro archivo style.css

```css
//fuente
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
```

{% hint style="info" %}
La buena practica en proyectos locales es descargar las fuentes e importarlas en el documento HTML.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 4.49.02 PM.png" alt=""><figcaption></figcaption></figure>

Vamos a usar la fuente en todo el documento, entonces vamos a usar el selector de etiqueta del body, para incluir nuestra fuente. Y removemos los otros selectores de etiqueta.

Te quedara algo así en tu archivo `style.css`

{% code lineNumbers="true" %}
```css
// styles

@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');

body {
  font-family: 'Open Sans', sans-serif;
}

```
{% endcode %}

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 4.51.01 PM.png" alt=""><figcaption></figcaption></figure>

## 2. Creemos un component Home

Vamos a crear nuestro primer componente.

Para ello vamos a crear algunas carpetas.

En react, existen diferentes formas de estructurar tu proyecto.&#x20;

* **src**: todos partes de una carpeta src, que seria la fuente, el origen.&#x20;

Existen carpetas como:

* **assets**, donde se guardan recursos como fuentes, imágenes, vectores, entre otras.
* **components**, donde se almacenan los componentes transversales a la funcionalidad de la aplicación. Es decir componentes/funciones, que puedas detectar se van a usar en muchos lugares de la aplicación. Puedes ser componentes presentacionales, que son componentes donde su función es mostrar contenido, y no incluye mucha lógica compleja detrás de escena.Se le conocen como **Stateless** o dump.&#x20;
* containers/pages/views, son generalmente los componentes que serán los que tendrán mas lógica, que tienen un manejo del estado, hacen peticiones, pueden ser también las paginas que se usaran en el enrutamiento. También se le conocen como componentes **Stateful** o smart.

Existen otras carpetas que el equipo pueda considerar si están manejando alguna librería adicional, para controlar el estado, o adicionales si usan typescript.&#x20;

{% hint style="info" %}
Typescript, era conocido como el superset de javascript. Ahora en la pagina oficial se le conoce como javascript con sintaxis para tipos.
{% endhint %}

Crearemos en nuestro proyecto dentro de la carpeta src, dos carpetas. Para ello sobre esta colocamos el mouse encima y damos click en el icono de la carpeta y crearemos la carpeta components

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.07.23 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.07.30 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.07.40 PM.png" alt=""><figcaption></figcaption></figure>

</div>

Damos enter, con el teclado y nos quedara la carpeta creada

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.12.54 PM.png" alt=""><figcaption></figcaption></figure>

Repetimos el mismo paso y crearemos una carpeta llamada pages

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.13.00 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.13.30 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.13.36 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.13.41 PM.png" alt=""><figcaption></figcaption></figure>

</div>

Dentro de pages vamos a crear el Home. Vamos a crear una carpeta llamada Home, siguiendo los mismos pasos anteriores.

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.16.39 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.16.46 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.16.52 PM.png" alt=""><figcaption></figcaption></figure>

</div>

Dentro de la carpeta crearemos 3 archivos. Un **index.js**, un archivo **Home.js** y **Home.style.css**

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.19.44 PM (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.19.52 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.19.57 PM.png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.20.02 PM (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.20.11 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.20.19 PM (1).png" alt=""><figcaption></figcaption></figure>

</div>

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.24.33 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.24.45 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 5.24.50 PM.png" alt=""><figcaption></figcaption></figure>

</div>

En el archivo Home vamos a crear una función, donde mostraremos un 'Hola Mundo', dentro de dos etiquetas **`<main></main>`**

importaremos en la primera linea la librería de React y luego crearemos la función. Como estamos trabajando con modulos de javascript para importarlos en otros archivos, es necesario exportar nuestra función, por lo que colocaremos la exportación por defecto, para que en nuestro index, podamos exportar nuestro componente.

````javascript
// Hola mundo
```javascript
import * as React from 'react';

const Home = () => {
  return <main>Hola Mundo</main>;
};

export default Home;

```a
````

Todo componente de react debe tener en la función return, obligatoriamente una etiqueta. Debe ser solo una y esta va a contener a todas las demás.

en el **`index.js`** vamos a realizar la exportación del componente Home.



````javascript
```javascript
export { default } from './Home';

```
````

Ahora vamos a importar nuestro componente en el componente padre App.



Borraremos las etiquetas internas y vamos a incluir la etiqueta del componente que seria en este caso `<Home>`, quedaria algo asi:



<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 10.05.29 PM.png" alt=""><figcaption></figcaption></figure>

## 3. Consumir una Api



Una Api (**A**pplication **P**rogramming **I**nterfaces), es un conjunto de definiciones y protocolos que se utiliza para desarrollar e integrar el software de las aplicaciones, **permitiendo la comunicación entre dos aplicaciones** de software a través de un conjunto de reglas. En este caso del Server vamos a llamar una información que vamos a mostrar en nuestra App.  La api que usaremos será la de Rick and Morty, y la vamos a incluir usando los hooks.

```typescriptreact
https://rickandmortyapi.com/api/character/?page=1
```

Para ello necesitamos usar el hook de `useEffect` y usaremos otros conceptos de javascript del asincronismo, el fecth.

Crearemos una función de `useEffect` y dentro vamos a crear una constante donde haremos uso del fetch para obtener la data.

Esto lo realizaremos en nuestro componente Home.

Ademas vamos a crear una variable de estado para almacenar la información que esta obteniéndose del llamado de Api.

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 10.19.38 PM.png" alt=""><figcaption></figcaption></figure>

{% code lineNumbers="true" %}
```javascript

import * as React from 'react';

const Home = () => {
  const [charactersList, setCharactersList] = React.useState([]);

  React.useEffect(() => {
    const list = fetch('https://rickandmortyapi.com/api/character/?page=1')
      .then((response) => response.json())
      .then((data) => setCharactersList(data.results))
      .catch(console.error);
  }, []);

  return (
    <main>
      Hola mundo
    </main>
  );
};

export default Home;

```
{% endcode %}

## 4. Mostrar la información del Api en el documento



Hasta este momento solo hemos hecho un llamado del Api, para mostrar la información. Vamos a borrar nuestro Hola mundo y a colocar un par de etiquetas para mostrar la información.



Dentro de las etiquetas `<main></main>`, vamos a incluir un titulo en un h1, una descripción en un párrafo y crearemos una sección donde en ella mostraremos una lista de elementos, en los cuales mostraremos una imagen del personaje de la serie, con el nombre y su especie.



{% code lineNumbers="true" %}
```html

  <h1 className="title">Este es el taller de React</h1>
  <p className="text">
    Para este taller vamos a usar el api de Rick and Morty
  </p>

```
{% endcode %}

Para el nombre con la imagen crearemos un `<div></div>` y dentro un `<picture></picture>`, con otras etiquetas y algunos atributos de clase, para mas adelante colocarle estilos.



{% code lineNumbers="true" %}
```html

   <div className="card">
    <picture className="card___image">
      <img src='imagen' alt='nombre' />
    </picture>
    <h3 className="card__title ">nombre</h3>
    <p className="card__text">
      species: <span>especie</span>
    </p>
  </div>

```
{% endcode %}



Como la idea es mostrar una lista de los personajes, entonces crearemos un componente en la carpeta components llamado Card.

Realizaremos los pasos que habíamos hecho antes para crear un componente.

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 10.29.56 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 10.30.10 PM.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 10.30.36 PM.png" alt=""><figcaption></figcaption></figure>

</div>

En el componente Card, vamos a crear una función, y en su contenido vamos a poner las etiquetas que habíamos creado para poner la información del personaje.&#x20;

Ademas como vamos a necesitar recibir la información del personaje, vamos a usar los props, como parámetro de nuestra función para obtenerlos. Esos parámetros le vamos a hacer un destructuring o destructuración.

{% hint style="info" %}
**Destructuring** o **destructuración**, es descomponer o desempacar los valores o propiedades de un array o un objeto. Por ejemplo:

\
const objeto1 = {\
&#x20; nombre: 'Ana',\
&#x20; edad: 5\
};\
\
//Destructuring\
const  { nombre, edad } = objeto1;\

{% endhint %}

Ademas de la destructuración, para mostrar las variables o en este caso el objeto con las propiedades que estamos obteniendo por los props, vamos a usar interpolación.

{% hint style="info" %}
**Interpolación**: es decirle a un elemento que va a incluir otro que puede ser de otra naturaleza. Por ejemplo para mostrar una variable en un atributo o en el jsx entre llaves, asignaremos el nombre.

```html
<img src={character.image} alt={character.name} />
```
{% endhint %}



{% code lineNumbers="true" %}
```javascript


import * as React from 'react';
import './Card.style.css';

const Card = ({ character }) => {
  return (
    <div className="card">
      <picture className="card___image">
        <img src={character.image} alt={character.name} />
      </picture>
      <h3 className="card__title ">{character.name}</h3>
      <p className="card__text">
        species: <span>{character.species}</span>
      </p>
    </div>
  );
};

export default Card;

```
{% endcode %}

Vamos a incluir nuestra Card en el componente Home.



En el Home, dentro de las etiquetas `<main></main>`, crearemos un `<section></section>` con atributos de clase.&#x20;

{% code lineNumbers="true" %}
```javascript

  <main>
    <section className="container___list">
    </section>
  </main>

```
{% endcode %}

Como el ideal es mostrar no un personaje, sino varios, entonces vamos a necesitar una lista y un iterador o ciclo como el array para que recorra la cantidad de elementos que estamos trayendo del api. Para incluir la lista usamos la interpolación y del array que queremos obtener los datos usamos el map y en su función vamo a crear los elementos `<li></li>` donde en ellos incluiremos la \<Card>. El componente `<Card />` es importante recordar que se debe importar.

{% code overflow="wrap" lineNumbers="true" %}
```javascript

  <main>
    <section className="container___list">
      <ul className="list">
        {charactersList.map((character) => (
          <li key={character.id}>
              <Card character={character} />
          </li>
        ))}
      </ul>
    </section>
  </main>

```
{% endcode %}

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 11.03.02 PM.png" alt=""><figcaption></figcaption></figure>

Si obtenemos un error como el anterior, importamos el Componente. Ademas es bueno importar la hoja de estilos.



{% code lineNumbers="true" %}
```javascript

import Card from '../../components/Card';

import './Home.style.css';

```
{% endcode %}

Podemos incluir algunos estilos para ver mas bonita nuestra aplicación.

## 5. Estilos para nuestros componentes

Si deseas incluir algunos estilos puedes usar los siguientes para las hojas del Home y de Card. Estos estilos pueden contener selectores adicionales, que es posible a este punto aún no hemos usado.

{% code title="Card.style.css" lineNumbers="true" %}
```css

.card {
  border: 0.1rem solid #3f51b5;
  border-radius: 1rem;
  cursor: pointer;
  opacity: 0.5;
}

.card:hover {
  opacity: 1;
}

.card___image > img {
  border-radius: 1rem 1rem 0 0;
  width: 100%;
}

.card__text {
  padding: 0.2rem;
}

.card__title {
  background-color: #3f51b5;
  color: wheat;
  margin: 0;
  padding: 0.8rem;
  text-align: center;
}


```
{% endcode %}



{% code title="Home.style.css" lineNumbers="true" %}
```css

.button {
  background-color: cornflowerblue;
  border: 0;
  border-radius: 0.5rem;
  color: white;
  cursor: pointer;
  font-weight: bold;
  margin-bottom: 1rem;
  padding: 0.5rem;
}

.button:hover {
  background-color: #3f51b5;
}

.title,
.list {
  align-items: center;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  list-style: none;
  padding: 0;
}

.list li {
  margin: 1rem;
}

.text {
  text-align: center;
}

.title {
  background-color: #3f51b5;
  border-radius: 0.5rem;
  color: wheat;
  padding: 1rem;
}


```
{% endcode %}

A este punto nuestro proyecto lucirá así:

<figure><img src="../.gitbook/assets/Screenshot 2023-03-10 at 11.12.41 PM.png" alt=""><figcaption></figcaption></figure>

{% embed url="https://react-haqcb4.stackblitz.io" %}

{% embed url="https://stackblitz.com/edit/react-haqcb4" %}



## 6. Seleccionando una Card y ocultando la lista (Extra)

Es posible que a este punto nos hayamos quedado sin tiempo. Pero un plus es que selecciones una carta, para ello usamos el evento click y al seleccionarlo vas a ocultar la lista usando los ternarios (condicionales) y mostrar solo el personaje seleccionado. Y al darle click en un botón para verlo todo, podrás nuevamente ver toda la lista de personajes.

Para esto puedes usar otra variable de estado, que te permita controlar la selección y otra que te guarde el elemento seleccionado.



### Resolviendo este extra



Vamos al elemento `<li></li>` a incluirle en evento click, para esto pondremos el atributo `onClick` y lo haremos igual a una función para manejar el click, que le pasaremos el objeto `character`.

{% hint style="info" %}
Los nombres de los eventos en React se debe usar con camelCase lowerCamelCase)
{% endhint %}

```javascript
<li
key={character.id}
onClick={() => handleSelectedCard(character)}
>

```

Vamos a definir la función handleSelectedCard y vamos a crear dos variables de estado; una variable para almacenar el eslemento seleccionado y la otra para saber si  se selecciono, entonces me guarde un true o false.

Primero vamosa crear las dos variables de estado:

{% code lineNumbers="true" %}
```javascript

const [isSelected, setSelected] = React.useState(false);
const [selectedCharacter, setSelectedCharacter] = React.useState(null);

```
{% endcode %}

Luego vamos a actualizar las variables de estado en la funcion que vamos a definir:

{% code lineNumbers="true" %}
```javascript

const handleSelectedCard = (character) => {
    setSelectedCharacter(character);
    setSelected(true);
};

```
{% endcode %}



Para mostrar nuestro elemento seleccionado, vamos a crear un elemento `<section></section>` y en el pondremos el componente `Card`, asignandole a la card en el prop del character, la variable de estado que creamos que tiene la info del personaje seleccionado. Ademas crearemos un botón con el texto "View All". Esta nueva sección va a quedar ubicado debajo de la anterior.



{% code lineNumbers="true" %}
```javascript
<section className="container__card">
  <button
    className="button"
    type="button"
  >
    View All
  </button>
  <Card character={selectedCharacter} />
</section>
```
{% endcode %}

En el caso de ser seleccionada una `Card` de la Lista nuestra sección nueva se mostrará,  junto con el nuevo botón, que tendra el texto de 'View All' y la lista se ocultará. Cuando se seleccione el botón, se mostrará de nuevo la lista y la sección de la `Card` seleccionada se ocultará.&#x20;

Entonces primero vamos a asignarle al boton el evento click, para que al seleccionarse cambie de estado, la nueva variable que creamos, para saber si el elemento se selecciono.

{% code lineNumbers="true" %}
```javascript

<section className="container__card">
    <button
      className="button"
      type="button"
      onClick={() => setSelected(false)}
    >
      View All
    </button>
    <Card character={selectedCharacter} />
  </section>

```
{% endcode %}

Ahora para mostrar o ocultar una sección solo nos falta preguntar por el valor del estado de la variable `isSelected`. Para preguntar por el valor, vamos a usar ternarios.

{% hint style="info" %}
**Ternarios**, los ternarios son operadores de javascript, que nos permiten hacer condicionales de javascript, pero cortos. Su sintaxis es la siguiente:

condicion ? expresión afirmativa : expresión negativa;
{% endhint %}

Vamos a meter las dos secciones en el ternario quedando así el código:



{% code lineNumbers="true" %}
```javascript

{!isSelected ? (
  <section className="container___list">
    <ul className="list">
      {charactersList.map((character) => (
        <li
          key={character.id}
          onClick={() => handleSelectedCard(character)}
        >
          <Card character={character} />
        </li>
      ))}
    </ul>
  </section>
) : (
  <section className="container__card">
    <button
      className="button"
      type="button"
      onClick={() => setSelected(false)}
    >
      View All
    </button>
    <Card character={selectedCharacter} />
  </section>
)}

```
{% endcode %}



## Codigo del extra



Aquí podrás ver el ejercicio completo de la aplicación en React (Aunque en esta ocasión se creo en stackblitz usando el React Typescript)

[https://taller-gdg-react.stackblitz.io/](https://taller-gdg-react.stackblitz.io/)

{% embed url="https://stackblitz.com/edit/taller-gdg-react" %}



