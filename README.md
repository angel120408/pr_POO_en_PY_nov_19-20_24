# Codigo #1 
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

print("Ramirez Torres Angel Msnuel De 3°W")
print("Num.Control : 1206")
print("Codigo #1")

#Inician los atributos 
class AlumnoDe3W:
    def __init__(self, alumno, calificacion):
        self.alumno = alumno
        self.calificacion = calificacion

    def imprimir_resultados(self):
        print(f"Alumno: {self.alumno}\nCalificación: {self.calificacion}")
        print("¡Has APROBADO!" if self.calificacion >= 7 else "¡Has REPROBADO!")

#Solicita los datos del alumno
nombre_alumno = input("Ingrese el nombre del alumno: ")
calificacion_alumno = float(input("Ingrese la calificación del alumno: "))

#Nos muestra los resultados 
alumno = AlumnoDe3W(nombre_alumno, calificacion_alumno)
alumno.imprimir_resultados()

![image](https://github.com/user-attachments/assets/50ee6e66-3d7e-4cd6-b551-16e0673cc443)
![image](https://github.com/user-attachments/assets/1428c363-c8b2-4834-a9fc-409307263aa4)

# Codigo #2
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

print("Ramirez Torres Angel Msnuel De 3°W")
print("Num.Control : 1206")
print("Codigo #2")

#Inicia la clase
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def cumpleaños(self, veces=1):
        self.edad += veces

#Solicita los datos del usuario
nombre = input("Ingrese el nombre: ")
edad = int(input("Ingrese la edad: "))

#Crea un objeto de la clase
persona = Persona(nombre, edad)

#Celebra dos cumpleaños
persona.cumpleaños(2)

#Nos muestra el resultado 
print(f"{persona.nombre} cumple {persona.edad} años")

![image](https://github.com/user-attachments/assets/177a0d64-bf96-4e6a-9983-0b2dfaaaf909)
![image](https://github.com/user-attachments/assets/ce68194b-d115-4466-badc-1c16b2d38fd1)

# Codigo #3
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

print("Ramirez Torres Angel Msnuel De 3°W")
print("Num.Control : 1206")
print("Codigo #3")

class Calculadora:
    def suma(self, num1, num2):
        #Aqui suma dos números y muestra el resultado
        return num1 + num2

    def resta(self, num1, num2):
        #Aqui resta dos números y muestra el resultado
        return num1 - num2

    def multiplicacion(self, num1, num2):
        #Aqui multiplica dos números y muestra el resultado
        return num1 * num2

    def division(self, num1, num2):
        #Aqui realiza una división, manejando la división por cero
        if num2 == 0:
            return "Error: No se puede dividir por cero."
        return num1 / num2


# Solicitar los números al usuario
num1 = float(input("Ingresa el primer número: "))
num2 = float(input("Ingresa el segundo número: "))

# Crear una instancia de la calculadora
calc = Calculadora()

# Realizando las operaciones
print(f"Suma: {calc.suma(num1, num2)}")
print(f"Resta: {calc.resta(num1, num2)}")
print(f"Multiplicación: {calc.multiplicacion(num1, num2)}")
print(f"División: {calc.division(num1, num2)}")

![image](https://github.com/user-attachments/assets/20e6db8d-eddd-4c9b-a974-f8bb4f55a13e)
![image](https://github.com/user-attachments/assets/659cb672-8887-427c-ad56-f980586088d0)
![image](https://github.com/user-attachments/assets/dabefac8-8456-4bb9-8faf-8036ac5bab2c)

# Codigo #4
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

print("Ramirez Torres Angel Msnuel De 3°W")
print("Num.Control : 1206")
print("Codigo #4")


class Persona():
    def __init__(self, nom, ape):
        #Pide el nombre y el apellido de la persona
        self.nombre = nom
        self.apellido = ape

    def nombre_completo(self):
        #Nos muestra el nombre completo de la persona
        print(self.nombre + " " + self.apellido)

#Clase Estudiante 
class Estudiante(Persona):
    def __init__(self, nom, ape, carr):
        #Llama a la clase base (Persona) para inicializar nombre y apellido
        super().__init__(nom, ape)
        self.carrera = carr

    def mostrar_carrera(self):
        print(self.carrera)

#Se crea la funcion principal donde solicita los datos al usuario 
def crear_estudiante():
    #Pedir nombre y apellido 
    nombre = input("Ingresa el nombre del estudiante: ")  # Solicita el nombre del estudiante
    apellido = input("Ingresa el apellido del estudiante: ")  # Solicita el apellido

    #Pide que ingreses tu carrera
    carrera = input("Ingresa la carrera del estudiante: ")  # Solicita la carrera del estudiante

    #Crear un objeto con los datos ingresados
    estudiante = Estudiante(nombre, apellido, carrera)
    
    # Mostrar el nombre completo y la carrera del estudiante
    estudiante.nombre_completo()  # Llama a la clase de Persona
    estudiante.mostrar_carrera()  #Llama a la clase de Estudiante

# Llamamos a la función para crear un estudiante
crear_estudiante()

![image](https://github.com/user-attachments/assets/26af9778-821f-437e-a2b2-d1f92391c4eb)
![image](https://github.com/user-attachments/assets/010f8dda-1994-46e7-ba7a-657376399f3c)
![image](https://github.com/user-attachments/assets/8216d79e-5abf-4108-8a6d-f71542d7b47e)


# Codigo #5
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

print("Ramirez Torres Angel Msnuel De 3°W")
print("Num.Control : 1206")
print("Codigo #5")

# Clase base que representa un vehículo genérico
class Fabrica:
    def __init__(self, llantas, color, precio):
        self._llantas = llantas
        self._color = color
        self._precio = precio

# Clase Moto, hereda de Fabrica
class Moto(Fabrica):
    def mostrar_datos(self):
        print(f"La cantidad de llantas: {self._llantas}")
        print(f"El color es: {self._color}")
        print(f"El precio es: {self._precio}")

# Clase Carro, hereda de Fabrica
class Carro(Fabrica):
    def mostrar_datos(self):
        print(f"La cantidad de llantas: {self._llantas}")
        print(f"El color es: {self._color}")
        print(f"El precio es: {self._precio}")

# Entrada de datos para Moto
print("Ingrese los datos para la moto:")
moto_llantas = int(input("Cantidad de llantas: "))
moto_color = input("Color: ")
moto_precio = input("Precio: ")
moto = Moto(moto_llantas, moto_color, moto_precio)

# Mostrar datos de Moto
print("\nOBJETO = moto")
moto.mostrar_datos()

# Entrada de datos para Carro
print("\nIngrese los datos para el carro:")
carro_llantas = int(input("Cantidad de llantas: "))
carro_color = input("Color: ")
carro_precio = input("Precio: ")
carro = Carro(carro_llantas, carro_color, carro_precio)

# Mostrar datos de Carro
print("\nOBJETO = carro")
carro.mostrar_datos()

![image](https://github.com/user-attachments/assets/9db256de-a557-4aba-ab8e-937e60a4235a)
![image](https://github.com/user-attachments/assets/c2b36cbb-50b0-40a8-bd9a-09ce70751b86)
![image](https://github.com/user-attachments/assets/6133899d-2d77-4404-9bd5-36e58fcb3942)

# Codigo #6
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

print("Ramirez Torres Angel Msnuel De 3°W")
print("Num.Control : 1206")
print("Codigo #6")

# Clase base para animales marinos
class Marino:
    def hablar(self):
        print("¡Hola, soy un animal marino!")

# Clase Pulpo que hereda de Marino
class Pulpo(Marino):
    def hablar(self):
        print("¡Hola, soy un pulpo!")

# Clase Foca que hereda de Marino
class Foca(Marino):
    def hablar(self, mensaje):
        print(mensaje)

# Crear instancias y mostrar sus mensajes
marino = Marino()
marino.hablar()

pulpo = Pulpo()
pulpo.hablar()

foca = Foca()
foca.hablar("¡Hola, soy una foca!")

![image](https://github.com/user-attachments/assets/70fcab73-d985-4fe8-9891-5fb48ca1fe00)
![image](https://github.com/user-attachments/assets/dfc8e331-2f96-400e-87e7-fdd46126d55d)
![image](https://github.com/user-attachments/assets/11e65d5c-b24a-4172-9035-d17b5c9c0bca)


# Codigo #7
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

# Clase que representa una universidad
class Universidad:
    def __init__(self, nombre):
        self.nombre_universidad = nombre

# Clase que representa una carrera universitaria
class Carrera:
    def __init__(self, especialidad):
        self.especialidad = especialidad

# Clase que representa un estudiante, hereda de Universidad y Carrera
class Estudiante(Universidad, Carrera):
    def __init__(self, nombre_universidad, especialidad, nombre_estudiante, edad_estudiante):
        Universidad.__init__(self, nombre_universidad)
        Carrera.__init__(self, especialidad)
        self.nombre = nombre_estudiante
        self.edad = edad_estudiante

    def mostrar_datos(self):
        print(
            f"El estudiante {self.nombre}, de {self.edad} años, "
            f"estudia {self.especialidad} en la universidad {self.nombre_universidad}."
        )

# Capturar datos del usuario
nombre_universidad = input("Ingrese el nombre de la universidad: ")
especialidad = input("Ingrese la especialidad de la carrera: ")
nombre_estudiante = input("Ingrese el nombre del estudiante: ")
edad_estudiante = int(input("Ingrese la edad del estudiante: "))

# Crear objeto estudiante y mostrar sus datos
estudiante = Estudiante(nombre_universidad, especialidad, nombre_estudiante, edad_estudiante)
estudiante.mostrar_datos()

![image](https://github.com/user-attachments/assets/7fc8bc31-b874-43a7-a86f-acee884c76bd)
![image](https://github.com/user-attachments/assets/3dfe7e46-0136-41c4-9bf0-78786aa11d04)
![image](https://github.com/user-attachments/assets/39e8336d-501c-4bdf-9373-819100552419)
