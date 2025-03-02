# RETO-8-POO
# Sistema de Gestión de Restaurante en Python

Este repositorio contiene un proyecto en Python que implementa un sistema de gestión de restaurante. El sistema incluye funcionalidades para gestionar múltiples órdenes, administrar el menú mediante persistencia en archivos JSON y recorrer los ítems de una orden utilizando un iterador personalizado.

## Características

- **Gestión de órdenes**:
  - Uso de una cola FIFO (con `deque`) para administrar y procesar las órdenes en el orden de llegada.
  
- **Gestión del menú**:
  - Creación, adición, actualización y eliminación de ítems en el menú.
  - Persistencia del menú en archivos JSON para mantener la información actualizada.
  
- **Estructura modular**:
  - Clases para representar distintos tipos de ítems del menú: *Beverage*, *Appetizer* y *MainCourse*.
  - Clase `Order` que gestiona la lista de platos, calcula totales y administra el menú.
  - Clase `Payment` para simular el procesamiento de pagos.
  - Clase `Restaurant` para manejar múltiples órdenes.
  
- **Iterador personalizado**:
  - Se implementa la clase `OrderItemsIterable` que permite recorrer todos los ítems de una orden de forma iterativa, devolviendo un diccionario con todos los atributos de cada ítem.

## Estructura del Proyecto

El proyecto se organiza en las siguientes clases:

- **MenuItem**:  
  Clase base para los ítems del menú, que contiene propiedades comunes como nombre y precio.

- **Beverage, Appetizer, MainCourse**:  
  Clases derivadas de `MenuItem` que añaden atributos específicos para bebidas, aperitivos y platos principales, respectivamente.

- **Order**:  
  Encargada de gestionar la lista de platos de una orden, calcular el total (aplicando descuentos en caso de tener un plato principal) y administrar el menú mediante persistencia en archivos JSON.

- **Payment**:  
  Simula el proceso de pago de una orden, mostrando el monto a pagar y el método de pago utilizado.

- **Restaurant**:  
  Utiliza una cola (FIFO) para gestionar y procesar múltiples órdenes de forma secuencial.

- **OrderItemsIterable**:  
  Permite recorrer de forma iterativa todos los ítems de una orden, devolviendo para cada uno un diccionario con todos sus atributos.
