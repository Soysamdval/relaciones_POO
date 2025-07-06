# 🧱 Composición en Programación Orientada a Objetos (POO)

La **composición** es una relación fuerte entre dos clases, donde **una clase está compuesta por otra**, y **si la clase principal desaparece, la contenida también**.

---

## 🚗 Ejemplo: Carro y Motor

```python
class Motor:
    def __init__(self, tipo):
        self.tipo = tipo

    def encender(self):
        print(f"Motor {self.tipo} encendido.")

class Carro:
    def __init__(self, marca, tipo_motor):
        self.marca = marca
        self.motor = Motor(tipo_motor)  # Composición: el motor nace dentro del carro

    def arrancar(self):
        print(f"Arrancando {self.marca}")
        self.motor.encender()
