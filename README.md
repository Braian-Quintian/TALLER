# Marco de trabajo D.D.D

## Domain Driven Design

## Diseño      Orientado  Dominio
  Entregable   Para que   Contexto 

//Va orientado al dominio para hacer el diseño

Monolito Trabaja todo
Microservicios trabajan una parte.

Domain-Drive-Design - Tackling 

Resuelve la demora con el testing

Arquitecto de software: Definir las necesidades del negocio
Ingenieria de software: Definir las mejores practicas para implementar

Restricciones drivers

Event storming es una metodologia paso 1 paso2 paso 3
Un marco no tiene por donde empezar

EL entregable de event storming es el Modelo de dominio

Para encontrar el dominio necesito hacer el taller de event Storming

Deuda técnica: vulnerabilidades, faltas

### Que estamos resolviendo

Eventos deben ir naranja

UI Blanco

Policy lola

Commando Azul

Aggregado amarillo

Cada color tiene su significado

## Que son los enventos de dominio

SUJETO + VERBO PASADO

## Fases

Fase 1  

Un pibote es un evento que si o si tiene que pasar


Cuando encuentras los eventos
salen los Hot spots y los conceptos
# Naranja es para eventos
Pago realizado
# Morado es para los temas que no se tienen claro, (Hot spots)
Como se va a pagar
# Amarillos son conceptos, se coloca la aclaracion
PSE, Tarjeta
# Azul es un comando puede disparar un evento
Verbo en presente + complemento sujeto

# Rosa es para el sistema externa
Por ejemplo:
Pago recibido, de quien? de paypal
Descargar archivo es un comando se descarga de S3 es un sistema externo

# Verde es listas que se necesitan para ejecutar el comando
Lista de peliculas -- Comando Elegir pelicula - Evento Seleccionada

# Colo lila es Politicas son reacciones a eventos de dominio especifico
va entre el evento y el futuro comando
Son las restricciones
Si usted reserva una silla 

## Amarillo GRANDE Agregado

Es quien recibe los comandos y decide si ejecuta o no , produciendo eventos de dominio
Agrupacion de eventos y comandos por responsabilidad

Las clases salen del flujo de negocio

## Conextos delitmitados 
El agrupamiento de agregados se separa por dominios

# Que es un microservicio
Un paquete tiene clases

Los comando son los metodos
Los eventos son las clases


Contextos delimitados:
Dominio core: LO que me hace diferente de los demas negocios

Dominio Soporte: Algo Que puedo desarrollar y apoya mi Core

Dominio Generico: Algo que puedo consumir o pagar "No lo desarrollo yo"

Siempre Debe haber Dominio core


Patrones de diseño y principios solid
