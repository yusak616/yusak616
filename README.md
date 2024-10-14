class Persona:
    # Constructor
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
   
    # Método utilizado al momento de imprimir el objeto o convertirlo en cadena (String)
    def __str__(self):
        return f"Mi nombre es {self.nombre} y tengo {self.edad} años"
   
    # Atributos
    nacionalidad =  "Mexicana"
 
    # Métodos o Funciones
    def obtenerNacionalidad(self):
        return f"Hola, soy {self.nombre} y soy de nacionalidad {self.nacionalidad}"
   
# Creación de objetos
carlos = Persona("Carlos", 25)
pedro = Persona("Pedro", 24)
valentina = Persona("Valentina", 40)
 
personas = [carlos, pedro, valentina]
for persona in personas:
    # Llamada al objeto, al ser utilizado de esta forma se convierte al objeto en texto, por lo que utiliza el método __string__
    print(persona)
 
    # Llamada al método obtenerNacionalidad() que regresa una cadena de texto (String)
    print(persona.obtenerNacionalidad())
