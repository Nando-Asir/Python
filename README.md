
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
```

- Usa `type()` para ver el tipo de dato.

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

---

## 4. Condicionales

```python
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
i = 0
while i < 5:
    print(i)
    i += 1
```

### for
```python
for letra in "Python":
    print(letra)
```

---

## 6. Funciones

```python
def saludar(nombre):
    print(f"Hola, {nombre}")

saludar("Carlos")
```

---

## 7. Listas, tuplas y diccionarios

### Listas
```python
frutas = ["manzana", "banana", "uva"]
```

### Tuplas
```python
punto = (4, 5)
```

### Diccionarios
```python
persona = {"nombre": "Luis", "edad": 25}
```

---

## 8. Manejo de errores (try/except)

```python
try:
    resultado = 10 / 0
except ZeroDivisionError:
    print("No se puede dividir por cero")
```

---

## 9. Módulos y paquetes

```python
import math
print(math.sqrt(16))
```

También puedes crear tus propios módulos guardando funciones en archivos `.py`.

---

## 10. Lectura y escritura de archivos

```python
# Escritura
with open("archivo.txt", "w") as f:
    f.write("Hola, archivo")

# Lectura
with open("archivo.txt", "r") as f:
    print(f.read())
```

---

## 11. Programación orientada a objetos

```python
class Persona:
    def __init__(self, nombre):
        self.nombre = nombre

    def saludar(self):
        print(f"Hola, soy {self.nombre}")

p = Persona("Lucía")
p.saludar()
```

---

## 12. Python avanzado (decoradores, generadores, etc.)

### Generadores
```python
def contador():
    i = 0
    while True:
        yield i
        i += 1
```

### Decoradores
```python
def decorador(func):
    def wrapper():
        print("Antes de la función")
        func()
        print("Después de la función")
    return wrapper

@decorador
def saludo():
    print("Hola")

saludo()
```

---

## 13. Proyectos prácticos

✅ Puedes crear una carpeta `proyectos/` con estos ejemplos prácticos:

- 🧮 **Calculadora en consola**
- 📁 **Gestor de tareas con archivos**
- 💸 **App de gastos personales (con JSON)**
- 🧠 **Juego de adivinar el número**
- 🌐 **API REST básica con Flask**

---

## 🚀 Contribuye o mejora este curso

¿Tienes ideas, ejercicios o mejoras? ¡Haz un pull request o crea un issue!

---

## 🧠 Recursos útiles

- [Documentación oficial de Python](https://docs.python.org/es/3/)
- [W3Schools Python](https://www.w3schools.com/python/)
- [Real Python](https://realpython.com/)

---

📄 **Licencia:** MIT  
✍️ Creado por Nando-Asir
