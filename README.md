# 2020-js-vanilla-testing-004

<p align="center">
    <img src="https://github.com/GeeksHubsAcademy/2020-geekshubs-media/blob/master/image/logo.png" >	
</p>


## Temario

* [Automatizando Tests en la nube](https://github.com/GeeksHubsAcademy/2020-js-vanilla-004/blob/master/README.md#)
* [Qué es un SaaS](https://github.com/GeeksHubsAcademy/2020-js-vanilla-004/blob/master/README.md#)
* [Travis-CI](https://github.com/GeeksHubsAcademy/2020-js-vanilla-004/blob/master/README.md#travis-ci)
* [Conclusiones](https://github.com/GeeksHubsAcademy/2020-js-vanilla-004/blob/master/README.md#conclusiones)
* [Referencias](https://github.com/GeeksHubsAcademy/2020-js-vanilla-004/blob/master/README.md#referencias)

### Automatizando Tests en la nube
```
Con el paso del tiempo, la evolución del Testing ha crecido mucho. El uso de herramientas para automatizar 
este paso de validación de código ha migrado del escenario local a la nube.

Muchas empresas otorgan servicios online gratuitos/pago para poder tener un entorno de pruebas continuado.
Permite que un proyecto desarrollado por un equipo, pueda sincronizar con un 'push' en git el lanzamiento
de las pruebas de manera automática en la nube.

Éste un paso muy rápido para validar el ciclo de vida de la aplicación y en resumidas cuentas es el inicio de
la integración continua aka CI.
```


### Qué es un SaaS
```
Es el acrónimo de 'Software as a Service'.
Un modelo de negocio que permite dar soporte lógico y de datos a traves de software ubicado en la nube.

Consiste en poder utilizar una aplicación desde nuestro cliente alojada en un servidor central.
Se delega toda la lógica y computación de datos en ésta última.

En resumidas palabras, la ejecución de una aplicación de nuestro local pero en la nube sin tener que
instalar nada y que se integra con otras aplicaciones online.

```

### Travis-CI

```
Es un sistema de Integración Continua, gratuita para proyectos Open-Source y de pago para proyectos privados.
Permite integrar sin problemas GitHub con la automáticamente de un 'pipeline' (test y build) en cada push o 
pull requests que hagamos al repositorio. 

Podemos decir que es una opción similar a Jenkins, pero tiene sus diferencias. No utiliza tareas programadas,
no tiene costos de mantenimiento (es un SaaS <[^_^]>! ) y su configuración es bastante fácil.
```

### Arquitectura del proyecto
```
La paquetería del proyecto ya esta definida por nosotros.

La raiz del repositorio contiene estos elementos:

/test
.gitignore
.travis.yml
package.json
package-lock.json
README.MD

En la carpeta 'test' encontrás 5 ficheros.

package.json
package-lock.json
suite.test.js
test04-toFixed.js
test04-toString.js

A nosotros solo nos interesan 

test04-toFixed.js
test04-toString.js
suite.test.js

El tercer fichero es la suite de Test que debemos de analizar.

 * test('toFixed(123456.52,5)  to equals "123456.52000" )', () => { ... }
 
 * test('toString(789) to equals "789" )', () => { ... }


Los dos primeros ficheros continene las funciones vacías que debemos implementar.

 * function toString(param) { return null; }

 * function toFixed(param,indice) { return null; }
 
```

### Convenio de trabajo
```
El proyecto ya está preparado para usar Travis automáticamente.

Cada alumno debe de tener una rama develop predefinida por el profesor para que puedas hacer PR's en ella.
Esto quiere decir, que si yo me llamo "T-1000", este repositorio debe de tener un rama 'develop_T-1000'.
Ésta servirá para subir los cambios. 

A Master no se va poder hacer PR's.

'Forkeate' el repo para que se genere una copia en tu cuenta local y puedas trabajar desde el mismo.
Arriba a la derecha, pulsa el botón 'Fork'.
```

![](https://github.com/GeeksHubsAcademy/2020-geekshubs-media/blob/master/image/2020-js-vanilla-testing-004/F00.png)

```
Una vez realizada la copia, ya puedes trabajar desde tu repositorio. 

Para probar si la implementación es correcta, debes de hacer una PR a la rama 'develop_{USER}' 
de GeekshubsAcademy.
```


```
Automáticamente, aparecerá un diálogo con un icono de Travis y el check del lanzamiento de los Tests.
```
![](https://github.com/GeeksHubsAcademy/2020-geekshubs-media/blob/master/image/2020-js-vanilla-testing-004/000.PNG)


### Conclusiones
```
ZZZZ
```


### Referencias
  * [Martin Fowler](https://martinfowler.com/articles/continuousIntegration.html)
  * [SaaS](https://es.wikipedia.org/wiki/Software_como_servicio)
  * [Travis-CI](https://docs.travis-ci.com/user/for-beginners/)
  


<div>
    <p align="center">
        <img src="https://github.com/GeeksHubsAcademy/2020-geekshubs-media/blob/master/image/pixel.png" >	
    </p>
  </div>
  
  <footer>
     <div>
        <a href="https://github.com/GeeksHubsAcademy/2020-js-vanilla-testing-003"><< Atrás</a>
         <a href="https://github.com/GeeksHubsAcademy/2020-js-vanilla-testing-004/blob/master/README.md#referencias">
        <img src="https://github.com/GeeksHubsAcademy/2020-geekshubs-media/blob/master/image/pixel.png" align="center"                  height="10" width="714"/>
         </a>
         <a href="https://github.com/GeeksHubsAcademy/2020-js-vanilla-testing-005">Siguiente >></a>   
    </div>
