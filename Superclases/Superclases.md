# 🏛️ Superclases en Programación Orientada a Objetos (POO)

Una **superclase** es una clase **general**, de la que otras clases más específicas **heredan atributos y métodos**.  
Sirve como **plantilla base** para organizar jerárquicamente el código y evitar repeticiones.

---

## 🚗 Ejemplo: Vehículo como superclase

```python
class Vehiculo:
    def __init__(self, marca):
        self.marca = marca

    def encender(self):
        print(f"{self.marca} está encendido.")

class Carro(Vehiculo):
    def tocar_claxon(self):
        print("¡Piiii!")

class Moto(Vehiculo):
    def hacer_caballito(self):
        print("¡Wiiii!")
