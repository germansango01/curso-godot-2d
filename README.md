# 🚀 Mi Primer Juego 2D con Godot

Este es un proyecto de práctica desarrollado siguiendo el tutorial oficial de Godot: **"Tu primer juego 2D"**.

El objetivo de este tutorial es enseñar los fundamentos de Godot 4, incluyendo la configuración de escenas, el movimiento del personaje, la generación aleatoria de enemigos (mobs) y la gestión de la lógica del juego.

## 🎯 Objetivo del Juego

El juego es un juego de esquivar donde el jugador (personaje) debe moverse para evitar a los enemigos (mobs) que aparecen en pantalla.

## 🛠️ Tecnologías Usadas

* **Motor de Juego:** Godot Engine 4.x
* **Lenguaje de Scripting:** GDScript

## 🖼️ Estructura de Escenas Principales

El proyecto consta de las siguientes escenas principales:

1.  **`Player.tscn`**: Contiene el código y los nodos para el personaje controlable.
2.  **`Mob.tscn`**: Contiene el código y los nodos para los enemigos que se mueven por la pantalla.
3.  **`HUD.tscn`**: Contiene la interfaz de usuario (mensajes, puntaje, temporizador).
4.  **`Main.tscn`**: Es la escena principal que orquesta el juego:
    * Genera instancias de `Mob`.
    * Controla el estado del juego (inicio, fin).
    * Conecta las señales del `Player` y `Mob` con el `HUD`.

## ⚙️ Características Implementadas (Seguimiento del Tutorial)

* **Movimiento del Jugador:** Implementación de la lógica de movimiento y colisiones.
* **Generación Aleatoria de Mobs:** Uso de un `Path2D` y `PathFollow2D` para crear rutas de movimiento para los enemigos que aparecen al azar.
* **Sistema de Puntuación:** Registro y visualización del puntaje del jugador.
* **Lógica de Game Over:** Manejo del fin del juego cuando el jugador es golpeado por un mob.
* **Música y Efectos de Sonido (Opcional):** Integración de audio para mejorar la experiencia.

## 🔗 Referencia del Tutorial

Puedes seguir el tutorial original aquí:
[https://docs.godotengine.org/es/4.x/getting_started/first_2d_game/index.html](https://docs.godotengine.org/es/4.x/getting_started/first_2d_game/index.html)