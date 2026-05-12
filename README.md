# BANDADA: Simulación de Comportamiento Emergente

Este proyecto es una implementación del algoritmo **Boids**, diseñado por Craig Reynolds en 1986. Simula el comportamiento colectivo de bandadas de aves, bancos de peces o enjambres de insectos, demostrando cómo reglas individuales simples pueden dar lugar a patrones grupales complejos y fluidos.

## 🦅 ¿Qué es el Comportamiento Emergente?

La emergencia ocurre cuando un sistema complejo exhibe propiedades que sus partes individuales no poseen. En esta simulación, ninguna "ave" (boid) sabe cómo formar una bandada; simplemente siguen tres reglas básicas respecto a sus vecinos locales, y la bandada "emerge" como resultado.

## ⚙️ Las Tres Reglas de Reynolds

El núcleo de la simulación se basa en tres fuerzas que actúan sobre cada individuo:

### 1. Separación (Evitar colisiones)
Cada boid intenta mantener una distancia mínima de sus vecinos para evitar chocar. Es una fuerza de repulsión local.

### 2. Alineación (Seguir al grupo)
Cada boid intenta volar en la misma dirección y a la misma velocidad que sus vecinos cercanos. Esto crea la sensación de una voluntad colectiva.

### 3. Cohesión (Permanecer unidos)
Cada boid intenta moverse hacia el centro de masa (la posición promedio) de sus vecinos. Esto evita que el grupo se disperse.

## 🛠️ Características del Laboratorio

- **Panel de Control en Tiempo Real:** Permite ajustar la intensidad de cada una de las tres reglas para observar cómo cambia el comportamiento social.
- **Variables Físicas:** Control de velocidad máxima, fuerza de giro, radio de percepción y evitación de bordes.
- **Interacción:** Posibilidad de atraer o dispersar a la bandada mediante el cursor.
- **Estética High-Tech:** Interfaz diseñada con una paleta de colores vibrante sobre fondo oscuro, optimizada para la visualización de partículas.

## 💻 Detalles de Implementación

- **Motor de Partículas:** Escrito en JavaScript puro utilizando el elemento `<canvas>`.
- **Cálculo Vectorial:** Uso de vectores para posición, velocidad y aceleración, permitiendo un movimiento suave y natural.
- **Optimización:** Gestión eficiente de ciclos de actualización para mantener una alta tasa de cuadros por segundo (FPS) incluso con cientos de boids.

## 🚀 Cómo ejecutarlo

Simplemente abre el archivo `index.html` en tu navegador o visita la [Demo en vivo](https://narquileerrado.github.io/bandada/).

---
*"El todo es más que la suma de sus partes."*
