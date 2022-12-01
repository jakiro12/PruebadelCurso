## Que es un Objeto en JavaScript
JavaScript está diseñado en un paradigma simple basado en objetos. Un objeto es una colección de propiedades y una propiedad es una asociación entre un nombre (o clave ) y un valor. El valor de una propiedad puede ser una función, en cuyo caso la propiedad se conoce como método .

Los objetos en Javascript permiten almacenar una gran cantidad de datos.

![](./imagenes/objectsExample.png)

<script>
    let myObj ={
        nombre: 'lauta',
        apellido:'carreño',
        desarrollador:true,
        edad: function calcAge(){ return 29},
        masInfo:{
            localidad:'santa fe'
        }
    }
    </script>

Los objetos pueden almacenar practiacmente cualquier tipo de dato, incluso pueden ser string almacenando otro string

<script>
    const saludo={
        'ejemplo':'hola'
    }
</script> // este caso es muy practico para almacenar infomarcion del tipo texto

Esta es la manera mas sencilla de crear objetos, tambien existen funciones/metodos propios de JS que permiten crear OBJ

<script>
    const lauta = new Object()
    lauta.name='lauta'
</script> //old mode, forma antigua de crear objetos


<script>
    const lauta = {
        nombre:'lauta'
    }
    const newLauta= Object.create(lauta)
</script>

<script>
      const lauta = {
    
    }
    const newLauta = Object.Assign(lauta,name:'lauta') //a quien le asigno y que le voy a meter dentro
</script>

![](./imagenes/crearObj.png) //Ejemplos

## Como acceder a su clave valor en los obj

*Dot Notation
Notacion de puntos, esta es relativamente la forma mas sencilla pero no dinamica
 <script>
    let objNew={
        name:'lauta'
    }
    console.log(objNew.name) //resultado 'lauta'
</script>

*bracket notation
Esta manera simula ser el llamado como si fuera una matriz, su ventaja es que es totalmente dinamica; se pueden pasar como parametros los valores

 <script>
    let objNew={
        name:'lauta'
    }
    console.log(objNew["name"]) //resultado 'lauta'
</script>