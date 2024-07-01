# MicroPython-ST7789V_TFT
MicroPython-ST7789V_TFT is a library created to use the "TFT Display ST7789V 240×320 SPI 2.4 in" module, available at [ST7789V UNIT ELECTRONICS](https://uelectronics.com/producto/modulo-tft-display-st7789v-240x320-spi-2-4%e2%80%b3-2-8/ "ST7789V UNIT ELECTRONICS") It is based on the work made by [rdagger](https://github.com/rdagger/micropython-ili9341 "rdagger").

The TFT Display ST7789V module, available in sizes of 2.4 and 2.8 inches, is an RGB screen with a resolution of 240x320. The communication protocol used for the screen is SPI.

![Modulo TFT Display ST7789V 240×320 SPI 2.4in](https://uelectronics.com/wp-content/uploads/2024/01/AR3950-Modulo-TFT-Display-ST7796S-SPI-2.4.jpg "Modulo TFT Display ST7789V 240×320 SPI 2.4in")

**Notes:**
- The original library was modified to fit the colors configuration of this screen.
- The tool for displaying images does not show the correct color gamma.

## What is a TFT Screen?
First, it is important to clarify that TFT is not a display technology; the term TFT refers to the type of transistors used in these screens, which improve image quality. Now that we know that TFT is not a display technology, we can say that unless otherwise specified, TFT screens usually use LCD display technology. This technology uses liquid crystal molecules placed between different layers that polarize and rotate according to the color to be displayed.

## Recommendations for using the TFT Screen
The screen needs to be programmed beforehand to display text or images.
Sometimes the development board is not enough to supply the necessary current for proper operation. If this is the case, we recommend connecting to a battery or another independent power source for the TFT screen.

# MicroPython-ST7789V_TFT
MicroPython-ST7789V_TFT es una librería creada para utilizar el modulo 'TFT Display ST7789V 240×320 SPI 2.4 in' disponible en [ST7789 UNIT ELECTRONICS](https://uelectronics.com/producto/modulo-tft-display-st7789v-240x320-spi-2-4%e2%80%b3-2-8/ "ST7789 UNIT ELECTRONICS") basada en el trabajo de [rdagger](https://github.com/rdagger/micropython-ili9341 "rdagger")

![Modulo TFT Display ST7789V 240×320 SPI 2.4in](https://uelectronics.com/wp-content/uploads/2024/01/AR3950-Modulo-TFT-Display-ST7796S-SPI-2.4.jpg "Modulo TFT Display ST7789V 240×320 SPI 2.4in")

El modulo TFT Display ST7789V disponible en tamaños de 2.4 y 2.8 in, es una pantalla RGB con una resolución de 240x320, el protocolo de comunicación utilizado para la pantalla es SPI 

## ¿Qué es una pantalla TFT?
Primero hay que aclarar que TFT no es una tecnología de visualización, el termino TFT se refiere al tipo de transistores que usan estas pantallas con los cuales se puede conseguir mejorar la calidad de las imágenes. Ahora que sabemos que TFT no es una tecnología de visualización , podemos decir que salvo que se especifique que la pantalla utiliza otro tipo de tecnología, las pantallas TFT suelen utilizar la tecnología de visualización LCD, la cual utiliza moléculas de cristal líquido colocadas entre diferentes capas que las polarizan y rotan según el color que se desea mostrar.

## Recomendaciones de Uso
La pantalla requiere ser programada previamente para poder mostrar texto/imagen
En ocasiones la tarjeta de desarrollo no es suficiente para poder suministrar la corriente para el buen funcionamiento, de ser así , te recomendamos realizar una conexión a una batería u otra fuente de alimentación independiente para la pantalla TFT.

**Notas:**
-La librería original fue modificada para adecuarse a los colores de ésta pantalla.
-La herramienta para mostrar imágenes no muestra la gamma correcta de colores.

# Original Project README:
# micropython-ili9341

MicroPython ILI9341 Display and XPT2046 Touch Screen Drivers

Full write-up on my website [Rototron](https://www.rototron.info/projects/esp32-pwned-password-checker/ "Rototron") or click the picture below for a YouTube video:

[![ILI9341 Tutorial](https://camo.githubusercontent.com/aedc68ee7874c4628fd7c166305842924355dfc9b837e27f19a89ac87235037b/68747470733a2f2f696d672e796f75747562652e636f6d2f76692f4e4a754f6b5353666755512f736464656661756c742e6a7067 "ILI9341 Tutorial")](https://www.youtube.com/watch?v=NJuOkSSfgUQ "ILI9341 Tutorial")

*Tested on ESP32 (Wemos Lolin32 & Loline32 Pro)*

**Notes:**

1. Use the img2rgb565.py tool located in the utils folder to convert image files like JPEG and PNG into the required raw RGB565 format.
2. The fonts available in this repository were made with a free conversion tool named [GLCD Font Creator](https://www.mikroe.com/glcd-font-creator "GLCD Font Creator").