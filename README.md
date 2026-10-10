# UnrealPinball

Title: Unreal Engine 3D Game - Pinball

Author: Fernando Arribas del Val

Date: 10/10/2026

Description: Práctica realizada para la asignatura de dispositivos y formatos. En ella hay que realizar mejoras funcionales y visuales al propio ejercicio entregado por el profesor.

Inputs: 

FlipperLeft: Hold and Release (mueve el flipper izquierdo arriba y abajo al presionar y soltar). Flecha derecha/GenericUSBController_Button1

FlipperRight: Hold and Release (mueve el flipper derecho arriba y abajo al presionar y soltar). Flecha izquierda/GenericUSBController_Button2

Launcher: Hold and Release (lanza la bola al presionar y soltar). Barra espaciadora/GenericUSBController_Button3

HitMachine: Pressed (golpea la máquina de pinball aplicando un pequeño impulso a la bola y generando un sacudido en la cámara). Number 0/GenericUSBController_Button4

Respawn: Pressed (permite cambiar la posición de la bola en la escena si esta se ha quedado atascada al punto de inicio - el lanzador). Flechas abajo/Flecha arriba/GenericUSBController_Axis1

Ball physical values and collisions:

Mass: 0,1 kg

Generate Overlap Events

Collisions: PhysicsActor

Friction: 0,05

Restitution: 1,0

Improve List:

. Modificación en la propiedad colisiones de la zona o parte "Wall902" de la mesa de pinball para que evite las colisiones, ya que tras probar diferentes valores para las físicas de la bola, esta siempre golpeaba con dicho objeto.

. Modificación en la propiedad colisiones de algunas de las zonas o partes "swXX" de la mesa de pinball para que evite las colisiones, ya que la bola se quedaba atascada en dichos objetos.

. Se añade un sistema de partículas de tipo niagara que se activa cuando el jugador alcanza una determinada puntuación (200 puntos por defecto) con efecto de monedas cayendo.

. Se añade un sistema de fin de partida cuando el jugador alcanza la puntuación máxima, saliendo del juego.

. Se añade un sonido que se activa cada vez que la bola golpea con alguno de los rebotadores.

. Se añade un texto para visualizar el sistema de puntuaje.

. Se añade una mejora visual al entorno añadiendo más elementos y cambiando la luminosidad de la escena. 

. Se añade un sistema de respawn al juego, tanto por pulsación de tecla (por si la bola cae fuera de la máquina de pinball) )como si la bola cae a la zona que hay debajo de los flippers.

. Se añade un sistema de temblor en la cámara del juego, simulando que el jugador golpea la máquina para mover la bola y redirigirla (se aplica un pequeño impulso a la bola).
