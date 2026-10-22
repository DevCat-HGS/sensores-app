# SensoresAPP — alerta temprana de inundaciones

Prototipo de alerta temprana de inundaciones con Arduino, hecho en equipo durante mi formación en el SENA. Unos
sensores de nivel miden el agua en tres alturas (bajo, medio y alto), y el sistema avisa con LEDs, una pantalla LCD
y el monitor serie. Un teclado con código protege el acceso al menú, un reloj RTC marca la hora de cada lectura y un
módulo Ethernet deja el estado disponible en la red local.

## Qué hay en cada carpeta

`archivos PP/` reúne las prácticas en el orden en que se construyó el prototipo:

| Carpeta | Qué prueba |
| --- | --- |
| `testdeinundacion0.1` → `1.0` | Lectura de los sensores de nivel y clasificación del riesgo |
| `LEDSPROTOTIPO`, `Pantalla`, `Display` | Indicadores: LEDs de colores y pantalla LCD |
| `Teclado`, `RELOJTECLADO`, `RTC` | Teclado con código de acceso y reloj de tiempo real |
| `PRACTICA_ETERNET1`, `practica_eternet2` | Publicar el estado por Ethernet |
| `PP`, `PP1.0`, `PP2` | El prototipo integrado, en tres versiones |

## Cómo probarlo

1. Abre la carpeta de la práctica en el IDE de Arduino.
2. Instala las librerías que pide cada sketch (`LiquidCrystal`, `Keypad`, `I2C_RTC`, `Ethernet`).
3. En los sketches con teclado, cambia el código de acceso (`password`) antes de instalar el equipo.

## Stack

Arduino (C++), sensores de nivel, LCD, teclado matricial, RTC por I2C y Ethernet por SPI.

---

Copia pública del código. Se dejaron fuera los documentos y entregas individuales de los integrantes del equipo.
