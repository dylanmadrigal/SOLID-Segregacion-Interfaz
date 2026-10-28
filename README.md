# SOLID-Segregacion-Interfaz
Ejemplo en C++ del Principio Segregación de Interfaz de SOLID

Este principio se implementa en la creación de interfaces pequeñas y especificas en lugar de una única interfaz general por asi decirlo.

Se definieron tres clases abstractas que actuan como interfaces especificas:
Enviable.h: Define la interfaz con el metodo puro enviar()
Remplazable.h: define la interfaz con el metodo puro reemplazar()
Expirable.h: define la interfaz con el metodo puro expirar()

En vez de forzar a la clase base producto a contener todos esos metodos, las clases derivadas heredan unicamnte las interfaces que realmente necesitan:
La clase Fisico hereda de Producto, Enviable y Remplazable, y la clase Digital implementa la interfaz Expirable
