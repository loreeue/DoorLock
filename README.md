# Sistema de Autenticación DoorLock

Este proyecto desarrolla un sistema de autenticación para abrir una puerta basado en tres niveles de seguridad: **APP**, **credenciales** y **huella dactilar**. Implementado como parte de la asignatura de Sistemas Empotrados y de Tiempo Real, este sistema combina software y hardware para garantizar la seguridad y la usabilidad.

En este [link](https://blogs.etsii.urjc.es/dseytr/sistema-de-autenticacion-en-una-puerta/) nos encontramos con una descripción más detallada del proyecto.

## Tabla de Contenidos
- [Introducción](#introducción)
- [Características](#características)
- [Componentes y Costos](#componentes-y-costos)
- [Casos de Uso](#casos-de-uso)
- [Problemas y Soluciones](#problemas-y-soluciones)
- [Requisitos del Sistema](#requisitos-del-sistema)
- [Configuración del Entorno](#configuración-del-entorno)
- [Ejecución](#ejecución)
- [Conclusión](#conclusión)

## Introducción
El **Sistema de Autenticación DoorLock** es una solución eficiente y segura que permite abrir una puerta únicamente a usuarios autorizados. Combina una placa Arduino Uno, un sensor de huella dactilar y una aplicación móvil para ofrecer triple autenticación.

Este sistema tiene múltiples aplicaciones, como en cuartos de servidores, oficinas o espacios donde la seguridad sea primordial.

## Características
- **Triple autenticación**: APP móvil, credenciales y huella dactilar.
- **Modo de alimentación dual**: USB o batería de 9V.
- **Pantalla LCD**: Muestra instrucciones y estados del sistema.
- **Eficiencia económica**: Coste competitivo frente a soluciones comerciales.

## Componentes y Costos
| Componente                 | Modelo         | Precio  |
|----------------------------|----------------|---------|
| Sensor de huella dactilar  | R307           | 24 €    |
| Módulo Bluetooth           | HC-05          | 10 €    |
| Motor Servo                | SM-S2309S      | 0 €     |
| Pantalla LCD               | 1802A          | 0 €     |
| Placa Arduino              | Elegoo UNO-R3  | 0 €     |
| Protoboard                 | -              | 0 €     |
| Maqueta 3D                 | -              | 45 €    |
| Spray                      | -              | 5 €     |
| Pines para cables          | -              | 15 €    |
| Materiales complementarios | -              | 18 €    |

**Total: 117 €**
*Coste reducido: Entre 54 € y 59 € utilizando materiales alternativos.*

## Casos de Uso
1. Añadir una nueva huella dactilar.
2. Autenticarse para abrir la puerta.
3. Visualizar mensajes y estados del sistema en la pantalla LCD.

## Problemas y Soluciones
- **Sensor de huella dactilar defectuoso**: Reemplazado por uno nuevo.
- **Cables sueltos**: Utilización de conectores adicionales.
- **Motor Servo roto**: Sustituido por otro disponible en el equipo.

## Requisitos del Sistema
- **Hardware**: Arduino Uno, sensor de huella dactilar, módulo Bluetooth, pantalla LCD, motor Servo.
- **Software**: IDE de Arduino, aplicación móvil desarrollada con MIT App Inventor.

## Configuración del Entorno
1. Conecta los componentes según el esquema del sistema.
2. Descarga e instala las librerías necesarias:
   - `Servo.h`
   - `LiquidCrystal.h`
   - `SoftwareSerial.h`
   - `Adafruit_Fingerprint.h`
3. Configura el módulo Bluetooth para la comunicación entre el Arduino y la aplicación móvil.

## Ejecución
1. Carga el código en la placa Arduino mediante el IDE correspondiente.
2. Enciende el sistema utilizando USB o batería de 9V.
3. Usa la aplicación móvil para interactuar con el sistema.

## Contribuidores en este proyecto

- [@alejandro](https://github.com/alejandroluzuriaga)
- [@oleksandr](https://github.com/DarkS34)
- [@yo](https://github.com/loreeue)


## Conclusión
El **Sistema de Autenticación DoorLock** es una solución innovadora que combina seguridad, usabilidad y bajo costo. Ofrece una alternativa viable a productos comerciales más costosos y representa una herramienta útil para entornos que requieren altos estándares de seguridad.
