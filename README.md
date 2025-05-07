
# Curso de Python desde Cero 🐍

Bienvenido/a a este curso gratuito y completo de Python para principiantes. Aquí aprenderás desde lo más básico hasta conceptos avanzados, con ejemplos prácticos y explicaciones claras. Ideal para estudiantes, autodidactas y futuros desarrolladores.

---

## 📚 Índice del curso

1. [Introducción a Python](#1-introducción-a-python)
2. [Variables y tipos de datos](#2-variables-y-tipos-de-datos)
3. [Operadores](#3-operadores)
4. [Condicionales](#4-condicionales)
5. [Bucles](#5-bucles)
6. [Funciones](#6-funciones)
7. [Listas, tuplas y diccionarios](#7-listas-tuplas-y-diccionarios)
8. [Manejo de errores (try/except)](#8-manejo-de-errores-tryexcept)
9. [Módulos y paquetes](#9-módulos-y-paquetes)
10. [Lectura y escritura de archivos](#10-lectura-y-escritura-de-archivos)
11. [Programación orientada a objetos](#11-programación-orientada-a-objetos)
12. [Python avanzado (decoradores, generadores, etc.)](#12-python-avanzado-decoradores-generadores-etc)
13. [Proyectos prácticos](#13-proyectos-prácticos)

---

## 1. Introducción a Python

### ¿Qué es Python?
Python es un lenguaje de programación interpretado, fácil de aprender, con una sintaxis clara y legible.

### Instalación
- Windows/macOS: [Descargar desde python.org](https://www.python.org/downloads/)
- Linux:
```bash
sudo apt install python3
```

### Tu primer script
```python
print("¡Hola, mundo!")
```

---

## 2. Variables y tipos de datos

```python
nombre = "Ana"         # Cadena
edad = 30              # Entero
altura = 1.65          # Float
es_estudiante = True   # Booleano

print(f"{nombre} tiene {edad} años y mide {altura}m")
```

---

## 3. Operadores

### Aritméticos
```python
x + y, x - y, x * y, x / y, x % y, x ** y, x // y
```

### Comparación
```python
x == y, x != y, x > y, x < y
```

### Lógicos
```python
and, or, not
```
### Ejemplo
```python
x = 10
y = 3

print(x + y)  # Suma
print(x % y)  # Módulo
print(x > y)  # Comparación
print(x > 5 and y < 5)  # Lógico
```

---

## 4. Condicionales

```python
edad = 20

if edad >= 18:
    print("Mayor de edad")
elif edad > 12:
    print("Adolescente")
else:
    print("Niño/a")
```

---

## 5. Bucles

### while
```python
i = 1
while i <= 5:
    print(f"Iteración {i}")
    i += 1
```

### for
```python
for numero in range(1, 6):
    print(f"Número: {numero}")
```

---

## 6. Funciones

```python
def multiplicar(a, b):
    return a * b

resultado = multiplicar(4, 5)
print("Resultado:", resultado)
```

---

## 7. Listas, tuplas y diccionarios

### Listas
```python
frutas = ["manzana", "banana", "uva"]
frutas.append("naranja")
print(frutas[1])
```

### Tuplas
```python
punto = (10, 20)
print("X:", punto[0])
```

### Diccionarios
```python
persona = {"nombre": "Luis", "edad": 25}
print(persona["nombre"])
```

---

## 8. Manejo de errores (try/except)

```python
try:
    numero = int(input("Introduce un número: "))
    print("Tu número es", numero)
except ValueError:
    print("Eso no es un número válido")
```

---

## 9. Módulos y paquetes

```python
import random

print("Número aleatorio:", random.randint(1, 100))
```

También puedes crear tus propios módulos guardando funciones en archivos `.py`.

---

## 10. Lectura y escritura de archivos

```python
# Escritura
with open("datos.txt", "w") as f:
    f.write("Línea 1\nLínea 2")

# Lectura
with open("datos.txt", "r") as f:
    for linea in f:
        print(linea.strip())
```

---

## 11. Programación orientada a objetos

```python
class Coche:
    def __init__(self, marca, modelo):
        self.marca = marca
        self.modelo = modelo

    def describir(self):
        return f"{self.marca} {self.modelo}"

mi_coche = Coche("Toyota", "Corolla")
print(mi_coche.describir())
```

---

## 12. Python avanzado (decoradores, generadores, etc.)

### Generadores
```python
def cuenta_regresiva(n):
    while n > 0:
        yield n
        n -= 1

for numero in cuenta_regresiva(3):
    print(numero)
```

### Decoradores
```python
def mayusculas(func):
    def envoltura():
        resultado = func()
        return resultado.upper()
    return envoltura

@mayusculas
def saludar():
    return "buenos días"

print(saludar())
```

---

## 13. Proyectos prácticos

- 🧮 **Calculadora en consola**
```python
def calcular():
    a = float(input("Número 1: "))
    b = float(input("Número 2: "))
    print("Suma:", a + b)

calcular()
```

- 🧠 **Juego de adivinar el número**
```python
import random

numero_secreto = random.randint(1, 10)
intento = int(input("Adivina el número (1-10): "))

if intento == numero_secreto:
    print("¡Correcto!")
else:
    print("Incorrecto, era", numero_secreto)
```

---

## 🚀 Contribuye o mejora este curso

¿Tienes ideas, ejercicios o mejoras? ¡Haz un pull request o crea un issue!

---

## 🧠 Recursos útiles

- [Documentación oficial de Python](https://docs.python.org/es/3/)
- [W3Schools Python](https://www.w3schools.com/python/)
- [Real Python](https://realpython.com/)
- [Tutorial Python en Español](https://docs.python.org/es/3.13/tutorial/index.html)

---

📄 **Licencia:** MIT  
✍️ Creado por Nando-Asir
