# Wokwi sn54act08 Chip

This is a custom chip for [Wokwi](https://wokwi.com/). It implements the sn54act08 IC.

## Description

The sn54act08 devices contain four independent 2-input AND gates. Each gate performs the Boolean function
of Y = (A . B)  in positive logic.

## Truth Table

| INPUT A | INPUT B |  OUTPUT |
| ------- | ------- | ------- |
|    H    |    H    |    H    |
|    L    |    X    |    L    |
|    X    |    L    |    L    |

## Pin names

| Name | Description              |
| ---- | ------------------------ |
|  1A  | Gate 1 Input signal  A   |
|  1B  | Gate 1 Input signal  B   |
|  2Y  | Gate 1 Output signal     |
|  2A  | Gate 2 Input signal  A   |
|  2B  | Gate 2 Input signal  B   |
|  2Y  | Gate 2 Output signal     |
|  3A  | Gate 3 Input signal  A   |
|  3B  | Gate 3 Input signal  B   |
|  3Y  | Gate 3 Output signal     |
|  4A  | Gate 3 Input signal  A   |
|  4B  | Gate 4 Input signal  B   |
|  4Y  | Gate 4 Output signal     |
| GND  | Ground                   |
| VCC  | Supply voltage           |


## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-sn54act08": "github:wokwi-custom-chips/sn54act08@0.1.0"
  }
```

Then, add the chip to your circuit by adding a `chip-sn54act08` item to the `parts` section of diagram.json:

```json
  "parts": {
    ...,
    { "type": "chip-sn54act08", "id": "chip1" }
  },
```

For a complete example, see [The sn54act08 chip test project](https://wokwi.com/projects/398983186186754049).
