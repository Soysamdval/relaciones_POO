#[he aquí el mapa conceptuaL:](./mapa_conpectual.png)
#[alt text](./UML.png)
# 🧬 Herencia en Programación Orientada a Objetos (POO)

La **herencia** es un principio fundamental de la Programación Orientada a Objetos (POO) que permite crear nuevas clases basadas en clases existentes.

Una **clase hija** (o subclase) hereda **atributos** y **métodos** de una **clase padre** (o superclase), evitando tener que escribir el mismo código varias veces. Además, la clase hija puede:

- Añadir nuevos métodos o atributos propios.
- Modificar el comportamiento de métodos heredados (lo que se conoce como *override* o *sobrescritura*).

Herencia permite **reutilizar código**, crear **jerarquías lógicas** (de lo general a lo específico) y escribir programas más **claros, mantenibles y escalables**.

---

## 📌 Ejemplo real

```python
class Animal:
    def __init__(self, nombre):
        self.nombre = nombre

    def comer(self):
        print(f"{self.nombre} está comiendo.")

class Perro(Animal):
    def ladrar(self):
        print(f"{self.nombre} dice: ¡Guau!")

