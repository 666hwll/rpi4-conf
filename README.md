# rpi4-conf

## using the raspberry pi 4 as a desktop machine
### with a chromebook level of performance

this config provides a overclocked pi, more allocated vram

and a powerbutton using gpio-shutdown on gpio3
the fan uses the second 5V Pin in the first row and the ground pin next to it
--> always on, as long as there is power
![Gpio-Header](IMG_0725.png)
![and where it's placed](IMG_0726.png)

that i how i build a powerbutton using a button with a digital signal lane, V And G

![Janky Wiring for Powerbutton](IMG_0633.jpeg)
![Button from the keyestudio smart home starter kit](IMG_0635.jpeg)

the button module is from the keyestudio smart home kit

