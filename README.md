# STM32H563ZI Calculator

## Description

This project is an embedded calculator built around the STM32H563ZI NUCLEO development board. It supports arithmetic on 8-digit positive integers using a 4×4 matrix keypad for input and a 16×2 character LCD for output. The calculator performs the four basic arithmetic operations—addition, non-negative subtraction, multiplication, and integer division—through dedicated keypad buttons while displaying results in real time on the LCD. The documentation below includes the keypad layout, operation mappings, GPIO pin assignments, power wiring information, and a complete bill of materials with links to the components used. Although the listed components were purchased from Mouser Electronics, equivalent parts from other suppliers can also be used.

---

## Button Layout

| 1 | 2 | 3 | A |
|---|---|---|---|
| 4 | 5 | 6 | B |
| 7 | 8 | 9 | C |
| * | 0 | # | D |


## Operations

| Button | Operation |
|--------|-----------|
| A | Addition |
| C | Non-Negative Subtraction |
| * | Multiplication |
| D | Integer Division |


## Pin Configurations

### Keypad

**GPIO Pins:**

- PB6
- PB7
- PG14
- PE13
- PE14
- PE11
- PE9
- PG12

### LCD Display

**Display Pins**

- PF3
- PD15
- PD14
- PB5
- PG9
- PA5
- PB9
- PB8

**Control Pins**

| Signal | Pin |
|--------|-----|
| Enable | PC3 |
| RW | PC0 |
| RS | PA6 |

## LCD Power

The power for the LCD display comes from an external 5V battery which is wired to a voltage regulator and potentiometer.
The output from the voltage regulator is wired to both the potentiometer and the LCD display power terminal V_DD, the output from the potentiometer is connected to the contrast termanal V_CC and controls the contrast behind each display box on the LCD.

---

## Parts

- [Board](https://www.mouser.com/en/ProductDetail/STMicroelectronics/NUCLEO-H563ZI?qs=Jm2GQyTW%2Fbjs0qOOBt6wkg%3D%3D)
- [LCD Display](https://www.mouser.com/en/ProductDetail/Newhaven-Display/NHD-0216BZ-RN-YBW?qs=kmv%2FWw32SUMqNraYmH1I%2Fw%3D%3D)
- [Keypad](https://www.mouser.com/en/ProductDetail/Parallax/27899?qs=qy7CnzY7nG6lIJGLMsv55A%3D%3D)
- [Battery Snaps & Contacts](https://www.mouser.com/en/ProductDetail/Keystone-Electronics/233?qs=jLI%2FJnmL0oAUrX2AwUR7sw%3D%3D)
- [Headers & Wire Housings](https://www.mouser.com/en/ProductDetail/Molex/22-28-4162?qs=GAPJcf4kvdthhmlVoo%252BzvQ%3D%3D)
- [Voltage Regulators](https://www.mouser.com/en/ProductDetail/Micro-Commercial-Components-MCC/MC7805CT-BP?qs=SdqRYZZ9IxChYPR4%2FIgmYA%3D%3D)
- [Potentiometer](https://www.mouser.com/en/ProductDetail/Bourns/3352T-1-103LF?qs=EYTJzGwugUoW6t2SAeQ12A%3D%3D)
- [Battery](https://www.mouser.com/en/ProductDetail/Panasonic-Battery/6LF22XWA-B12?qs=8uu3sA0mUdvMhS%2FBFiaz%252BQ%3D%3D)
- [Breadboard](https://www.mouser.com/en/ProductDetail/BusBoard-Prototype-Systems/BB830?qs=VEfmQw3KOauhPeTwYxNCaA%3D%3D)
- [Capacitors](https://www.mouser.com/en/ProductDetail/KEMET/T350A104K035AT?qs=O4djsYW3GvYvdg%2Fd42QtNw%3D%3D) (Optional, for use in conjunction with the voltage regulator)

---

## Notes

- All parts were purchased from mouser electronics and the links above reflect that, the same or similar parts may be available for purchase from other sources.
- Mouser does not sell an LCD display that has pre-connected header pins, the headers & wire housing would need to be soldered onto the LCD display.
- I did not include it above but it should go without saying that you will need male to male wires but they are fairly common and can be purchased from a variety of sources.