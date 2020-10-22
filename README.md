# Smart Home
![](/img/smartHomes3.png)
![](/img/GT000002.svg)


Dispositivo diseñado para taller práctico de Internet de las Cosas aplicado a dómotica durante el FIT (Foro de Innovación Tecnológica). Evento organizado por Universidad Galileo en Guatemala. 
El dispositivo contiene:
- ESP32
- Acelerómetro
- Sensor de intensidad de luz
- NeoPixeles
- Buzzer
- BME280
- Control de cargas AC.

# ¿Quién obtuvo un Smart Home?

Los participantes ganadores del mejor proyecto en el taller práctico de Internet de las Cosas obtuvieron su tarjeta electrónica Smart Home.

# ¿Cómo funciona?

El Smart Home funciona por medio de un microcontrolador ESP32 el cual posee conectividad WiFi y BLE, el cual puede ser programado con difentes lenguajes de programación entre los mas utilizados se encuentra C++ y Micropython.

# ¿Qué podemos hacer?

Pesplegar información por medio de un web server o dashboard MQTT en plataformas como [adafruitIO][adafruit_io] por medio de conexión WiFi, obtiene mediciones de temperatura, humedad y presión atmosférica por medio del sensor BME280, podemos controlar cargas AC por medio de sus Relay, cuenta con LED de tipo NeoPixel como indicadores, Buzzer para aplicaciones con sonido y es capas de ser conectada con asistentes de voz como Alexa y google assistant.

[adafruit_io]: https://io.adafruit.com

# Ejemplos con MicroPython 

Para utilizar micropython con nuestro Smart Home visite el siguiente repositorio para mayor información  [FunPython Ecuador][FPE].

[FPE]: https://github.com/FunPythonEC/FIT_Guatemala_2019-SMART_HOME

# Descripción de pines 

### Temperatura, humedad y presión atmosférica - Comunicación I2C
ESP32 | BME280
--- | ---
SCL 22 | SCK 4
SDA 23 | SDI 3

### Acelerómetro/Giróscopio - Comunicación I2C
ESP32 | MMA8425QT
--- | ---
SCL 22 | SCL 4
SDA 23 | SDA 6

### RELÉ
ESP32 | Relé Derecha | Relé Izquierda
--- | --- | ---
PIN ESP32| GPIO 13 | GPIO 12


### NEOPIXEL - Comunicación SPI
ESP32 | PIN
--- | ---
5V | VCC 
GND | GND
GPIO 15 | DIN

### LIGHT SENSOR
ESP32 | ALS-PT19-315C
--- | ---
GPIO 2 | ADC 

### BUZZER
ESP32 | BUZZER
--- | ---
GPIO 14 | DIN

# Licencia

Hardware License: CERN OHL v1.0 para más información visitar el siguiente [Link][CERN_v1].

[CERN_v1]: https://ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-1.2

Software License: GPL v3

Documentation License: CC BY 4.0 International
