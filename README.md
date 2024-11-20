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









# Codigo #6
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY








# Codigo #7
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

