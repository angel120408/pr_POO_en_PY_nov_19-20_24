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

class Calculadora:
    def suma(self, num1, num2):
        """Suma dos números y muestra el resultado."""
        return num1 + num2

    def resta(self, num1, num2):
        """Resta dos números y muestra el resultado."""
        return num1 - num2

    def multiplicacion(self, num1, num2):
        """Multiplica dos números y muestra el resultado."""
        return num1 * num2

    def division(self, num1, num2):
        """Realiza una división, manejando la división por cero."""
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

![image](https://github.com/user-attachments/assets/8c0791cd-def2-4cd3-a746-6b8fc5129cc5)
![image](https://github.com/user-attachments/assets/a3f66269-ff26-46fd-a3ef-6fc85b16cbc6)
![image](https://github.com/user-attachments/assets/dabefac8-8456-4bb9-8faf-8036ac5bab2c)

# Codigo #2
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY








# Codigo #2
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY









# Codigo #2
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY








# Codigo #2
- codigo creado con el ejemplo del codigo #1 de los ejercicios de PY

