# 🌀 Polimorfismo en Programación Orientada a Objetos (POO)

El **polimorfismo** permite que diferentes clases implementen un mismo método de manera distinta.  
Significa “muchas formas” y le da **flexibilidad** al software.

---

## 🐕 Ejemplo: Perro y Gato

```python
class Animal:
    def hacer_sonido(self):
        pass

class Perro(Animal):
    def hacer_sonido(self):
        print("¡Guau!")

class Gato(Animal):
    def hacer_sonido(self):
        print("¡Miau!")

animales = [Perro(), Gato()]

for animal in animales:
    animal.hacer_sonido()
