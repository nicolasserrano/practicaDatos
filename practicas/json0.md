# Ejemplo 0 JSON

Se va a crear un objeto JSON, que es el que se utiliza en el Ejemplo 1.  
Para ello abrir la consola del navegador, pulsando la tecla F12 y seleccionar la pestaña "Console".
Si muestra algún mensaje se puede borrar con las teclas Ctrl + L

Crear un objeto de nombre obj con la sentencia:
> obj={}

Añadir los atributos name y age con los siguientes valores:
> obj.name = "sofia"
> obj.age = 30

Añadir un nuevo atributo pets que va a contener un array.
> obj.pets = []

Se van a añadir 3 elementos a dicho array. Cada elemento es un objeto, por lo que los creamos:
> obj.pets[0] = {}
> obj.pets[0].animal = "dog"
> obj.pets[0].name = "Fido"
> obj.pets[1] = {}
> obj.pets[1].animal = "cat"
> obj.pets[1].name = "Felix"

y el tercer elemento lo añadimos con la sintaxis:
> obj.pets[2] = {"animal":"hamster","name":"Lightning"}

Se puede ver el contenido de obj al teclear:
> obj

Se puede convertir a texto con:
> JSON.stringify(obj)

y guardar en una variable de texto con:
> objText = JSON.stringify(obj)

Y crear el objeto a partir de la variable texto con:
> obj2 = JSON.parse(objText)

Se proporcionan todos los comandos unidos a continuación:
<textarea>
obj={}
obj.name = "sofia"
obj.age = 30
obj.pets = []
obj.pets[0] = {}
obj.pets[0].animal = "dog"
obj.pets[0].name = "Fido"
obj.pets[1] = {}
obj.pets[1].animal = "cat"
obj.pets[1].name = "Felix"
obj.pets[2] = {"animal":"hamster","name":"Lightning"}
obj
JSON.stringify(obj)
objText = JSON.stringify(obj)
obj2 = JSON.parse(objText)
</textarea>
