# 🧩 Agregación en Programación Orientada a Objetos (POO)

La **agregación** es una relación de contención entre clases donde una clase "todo" contiene a otras, pero **sin ser completamente responsable de su existencia**.

---

## 🎓 Ejemplo: Salón de clases y Estudiantes

```python
class Estudiante:
    def __init__(self, nombre):
        self.nombre = nombre

    def presentarse(self):
        print(f"Hola, soy {self.nombre}")

class SalonDeClases:
    def __init__(self, numero):
        self.numero = numero
        self.estudiantes = []

    def agregar_estudiante(self, estudiante):
        self.estudiantes.append(estudiante)

    def mostrar_estudiantes(self):
        for est in self.estudiantes:
            est.presentarse()
