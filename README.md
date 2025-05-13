# rpi4-conf
-------------------------------------------
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
--> the button only works this way, because it is getting 3V to V(U) and gpio3 as S
(Ground is Ground ofc)

## Operating System?

Versions of Android (for example the one by Emteria) or Linux Distros (Ubuntu, Raspberry Pi OS, Manjaro, ... )

## What Desktop Environment or Window Manager to choose?

The default desktop of RaspberryPiOS is not the only choice --> 

1. DWM or DWL; for the tech savy (WM):
    Those desktops are configured and compiled using the C programming language; meaning the performance is pretty 
    good by default, even if the standart features aren't exactly overwhelming. 
    Pros:
        - Can work with less than 256 mb --> perfect for embedded projects like kiosks and tech elitists
        - There are forks and configurations by the community that make it work like a DE (JWM for example) 
    Cons:
        - You NEED to know the C Language
2. Xfce; Balanced and solid option (DE):
    A lightweight desktop with nearly all the features you'd miss from KDE and Gnome.
    Works with weaker hardware.
    Pros:
        - Good Defaults
    Cons:
        - Nothing really special
3. i3 or sway; for Intermediate Users (WM):
    Both are battle-tested and alright; but especially keyboard binds can be a real struggle if you don't use
    an American English Keyboard layout --> which sucks. 
    Pros:
        - Stable and medium sized community
    Cons:
        - Faible for American English Layouts
4. LXQT; the Lightweight Alternative (DE):
    Like the default RasperryPiOS Desktop but less polished with better performance.
    Pros:
        - Does the core features you'd want really well
    Cons:
        - Customization can destroy the advantage of the resource management 

Inspiration: <https://www.stoffl.net/2020/03/31/how-to-raspberry-pi-4-gpio-ein-und-ausschalten-power-on-off-button/>