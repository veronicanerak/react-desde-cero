# La mejor manera de empezar con React

## 1. Las virtudes de thinking in react como tutorial

Para empezar a sumergirse en el mundo ***React*** basemonos en la documentacion oficial de [React](https://facebook.github.io/react/docs/thinking-in-react.html?) Donde sustenta los ejemplos con los conceptos claros y faciles de entender. Adicionalmente usa **Codepen** el cual permite ejecutar el codigo y poder editarlos viendo los resultados al mismo tiempo. De esa manera ejecutar ejemplos desde el primer momento lo cual facilita su comprencion.

## 2. Como ejecutar en codepen
Es muy intuitivo ejecutar codigo usando **codepen** Ejemplo [veamos](http://codepen.io/rohan10/pen/qRqmjd):
Podemos agregar contenido en cualquier seccion y ver el resultado en la region inferior.
![Editando codigo en codepen](https://github.com/veronicanerak/react-desde-cero/blob/master/thinking-in-react-codepen.png)

## 3. Como exportar y correr ejemplos de codepen en tu computadora
    * Exportar el codigo: Click en el boton `Export`
![Exportar codigo de codepen](https://github.com/veronicanerak/react-desde-cero/blob/master/export-codepen-code.png)
    * Descomprimir lo que acabamos de exportar, tendremos la siguiente estructura:
![Estructura ejemplo codepen](https://github.com/veronicanerak/react-desde-cero/blob/master/codepen-structure.png)
 Click en: index.html (el archivo principal de la aplicacion)
    * Hecho, ya vemos el ejemplo corriendo correctamente
![proyecto Codepen](https://github.com/veronicanerak/react-desde-cero/blob/master/codepen-example.png)

## 4. Por que no se puede editar?
Si intentaste editar los archivos te habras dado cuenta que no es posible editar porque el archivo `js/index.js` es el archivo javascript con el codigo ya `traspilado/compilado` por [Babel](https://babeljs.io/) Que es el compilador de JavaScript. Es decir no tenemos el codigo original para editarlo. 

## 5. Paso a paso como pasarlo a create react app

>Para ejecutar el ejemplo anterior con `create-react-app` seguir los siguientes pasos: 

1. Crear la aplicación ejecutando:
    `create-react-app nombre_aplicacion`

2. Levantar el servicio, ingresar a nombre_aplicacion y ejecutar:
    `cd nombre_aplicacion`
    `yarn start`

3. Hacer correr la aplicación de: [codepen](http://codepen.io/rohan10/pen/qRqmjd) 
![Codepen estructura del proyecto](https://github.com/veronicanerak/react-desde-cero/blob/master/convert-to-create-app-react.png)
Para ello seguir los siguientes pasos:
    * Abrir la aplicación creada y copiar el contenido de HTML en:   
  		`nombre_aplicacion/public/index.html`

    * Copiar el contenido de CSS en:
		`nombre_aplicacion/src/App.css`

    * Copiar JS en:
        `nombre_aplicacion/src/App.js`

    * Ejecutar:  
         `yarn start`
en la consola se vera muchos errores, como vemos en la siguiente imagen . Sin asustarse importando los archivos faltantes y algun otro cambio lo solucionamos.
![Errores codepen](https://github.com/veronicanerak/react-desde-cero/blob/master/errors-compile.png)

4. Empezamos a corregir los errores:
    a) Importar React. Agregar en el archivo:  `nombre_aplicacion/src/App.js` en la linea 1
		`import React, { Component } from 'react';`

    b) Si vemos la jerarquía de los componentes vemos que el componente principal es: `FilterableProductTable`. Revisemos el archivo 	 
    	`nombre_aplicacion/src/index.js`
	![Jerarquía de los componentes](https://github.com/veronicanerak/react-desde-cero/blob/master/codepen-estructura-componentes.png)
	

    c) Importamos el componente principal reemplazando App por `FilterableProductTable` (que es el componente principal)  (Ver la siguiente imagen)
    ![Codepen reemplazar componente](https://github.com/veronicanerak/react-desde-cero/blob/master/replace-main-component.png)
    
    d) Importamos `ReactDOM`. Ir al archivo `nombre_aplicacion/src/App.js`
 		y agregar en la linea 2: 
		`import ReactDOM from 'react-dom';`
	e) Importamos el archivo que contiene los estilos. En el mismo archivo `nombre_aplicacion/src/App.js`
agregar en la linea 3:
		`import './App.css';`

6. Hecho! 
    Ejecutar yarn start (si no lo hizo anteriormente)
    y puede aver la aplicación funcionando correctamente en el navegador:
    ![Proyecto react](https://github.com/veronicanerak/react-desde-cero/blob/master/thinking-in-react-mock.png)




	
