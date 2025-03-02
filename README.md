# Restaurant Order Management System

Este repositorio contiene un proyecto en Python para la gestión de pedidos en un restaurante. Se implementa un sistema de menú y órdenes, que incluye clases para representar diferentes tipos de ítems (bebidas, aperitivos y platos principales), además de funcionalidades para gestionar el menú (crear, actualizar, eliminar y guardar en un archivo JSON) y para procesar órdenes y pagos.

## Características

- **Clases de ítems de menú:**  
  - **MenuItem:** Clase base con atributos comunes.
  - **Beverage, Appetizer, MainCourse:** Clases derivadas que extienden a *MenuItem* y añaden atributos específicos.
  
- **Gestión de Menú:**  
  Permite cargar, guardar y modificar el menú usando un archivo JSON.

- **Gestión de Pedidos y Pagos:**  
  Permite agregar platos a un pedido, calcular el precio total (incluyendo descuentos) y procesar pagos.

- **Iterador de Ítems del Pedido:**  
  Se implementa la clase `OrderItemsIterable` que permite recorrer de manera iterativa todos los ítems de un pedido, devolviendo un diccionario con todos sus atributos.

- **Cola de Órdenes:**  
  La clase `Restaurant` utiliza una cola para gestionar múltiples órdenes de manera secuencial.

## Uso

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/tu_usuario/restaurant-order-system.git
   cd restaurant-order-system
Ejecutar el código:

El archivo principal contiene ejemplos de uso para cada funcionalidad. Para ejecutarlo:

bash
Copiar
Editar
python main.py
Modificar el menú:

Puedes agregar, actualizar o eliminar ítems del menú editando el archivo menu.json o utilizando los métodos correspondientes en la clase Order.

Iterar sobre los ítems de un pedido:

Utiliza la clase OrderItemsIterable para recorrer todos los elementos de una orden y obtener sus atributos.

Estructura del Proyecto
main.py: Archivo principal que contiene la implementación completa y ejemplos de uso.
menu.json: Archivo para guardar y cargar el menú del restaurante.
README.md: Este archivo.
Requisitos
Python 3.x
