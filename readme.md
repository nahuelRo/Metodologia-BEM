# Metodologia en CSS

1. Los problemas en CSS
2. Metodología y Arquitectura
3. Metodologia vs Arquitectura
4. Qué es una metodología en CSS?
5. Metodología BEM

# Los problemas en CSS

Los problemas más comunes de CSS son:
* 👉 Mala prácticas como selectores, especificidad...
* 👉 Qué nombre le pongo a una etiqueta?

Y para solventar este problema existen varias soluciones como:
* 👉 Básicas (Header, Wrapper..)
* 👉 Metodologías

# Metodología y Arquitectura

Cuando queremos definir como equipo cómo se desarrollará el proyecto nos encontramos que debemos definir:
* 👉 Estructura del CSS (Arquitectura)
* 👉 Cómo trabajar CSS (Metodología)

Y tienen como objetivo cumplir con CSS sea:
* 👉 Comprensible
* 👉 Predecible
* 👉 Reutilizable
* 👉 Escalable
* 👉 Modular


# Metodología vs Arquitectura

Como resumen rápido:
* 👉 Arquitectura se centra en la organización de carpetas.
* 👉 Metodología se centra en cómo nombrar las clases.

👁️ Cuidado!
* Aunque en el día a día, blogs o tutoriales muchas veces se le llama metodología a una arquitectura o viceversa simplemente por comodidad.

# Qué es una metodología en CSS?

Una metodología es un método a seguir para conseguir un objetivo en concreto.

El objetivo en CSS es ponele nombre a las clases y en términos generales se pueden dividir en dos "conceptos":
* 👉 Bloque o Estructura
* 👉 Funcionalidades o Herramientas


# Metodología BEM

## Qué es BEM?
Es una metodología que se centra en el concepto de bloque o estructura.

Es decir las reglas cómo definir clases se basa en la estructura de HTML teniendo en cuenta:
* 👉 Bloque es la **contenedora**
* 👉 Elemento son las **Hijas** de la **contenedora**
* 👉 Modificador son **Hijas** con la propiedades diferentes

Web oficial: [https://getbem.com/](https://getbem.com/)

## Sintaxis de BEM
Sólo se usan class, nada de id.
Los nombres de las clases no usan ningún tipo de nomenclatura como Pascal Case o Kebab Case.

Y su sintaxis se basa en:

|          | Carácter | Sintaxis |
|----------|----------|----------|
| Bloque   |          | .bloque   |
| Elemento |    __    | .bloque__elemento   |
| Modificador    |    --    | .bloque__elemento--modificador   |


## Ejemplo de BEM
Aquí tienes un ejemplo de HTML con BEM


```html
<div class="bloque">
  <div class="bloque__elemento"></div>
  <div class="bloque__elemento bloque__elemento--modificador"></div>
</div>
```

```html
<div class="menu">
  <div class="menu__li"></div>
  <div class="menu__li  menu__li--active"></div>
</div>
```

Aquí tienes un ejemplo en CSS con BEM

```css
.menu{}
.menu__li{}
.menu__li--active{}
```

##  Ventajas vs Desventajas de BEM
BEM tiene muchas ventajas en el código de día a día:
* 👉Los nombres de las clases en CSS son fáciles
* 👉Muy pensados para usar con preprocesadores (SCSS)

Pero también algunas "desventajas":
* 👉 El HTML queda muy largo



