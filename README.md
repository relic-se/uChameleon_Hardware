# μChameleon Hardware
Digital guitar effects pedal designed around the Raspberry Pi Pico 2 and the TLC320AIC3204.

| 3D Enclosure | PCB Top | PCB Bottom |
|-|-|-|
| ![3D rendering of μChameleon assembled enclosure](assets/enclosure.png) | ![3D rendering of the top of the μChameleon PCB](assets/pcb-top.png) | ![3D rendering of the bottom of the μChameleon PCB without a Raspberry Pi Pico 2](assets/pcb-bottom.png)

## Software

- [CircuitPython Firmware](https://github.com/relic-se/uChameleon_CircuitPython)
- Arduino Firmware _(planned)_

## GPIO Configuration

The following table defines the pin configuration for the Raspberry Pi Pico (1 or 2) device.

| Pin | Function | Name | Description |
|-----|----------|------|-------------|
| GP0 | UART | MIDI_OUT | MIDI output at 31.25 kHz |
| GP1 | UART | MIDI_IN | Opto-isolated MIDI input at 31.25 kHz |
| GP2 | I2C | SDA1 | STEMMA QT data input/output |
| GP3 | I2C | SCL1 | STEMMA QT clock |
| GP4 | GPIO | RST | Codec reset output _(active low)_ |
| GP5 | I2S | MCLK | Master clock |
| GP6 | I2S | BCLK | Bit clock |
| GP7 | I2S | WCLK | Word clock |
| GP8 | I2S | DOUT | Digital audio data out (DAC) |
| GP9 | I2S | DIN | Digital audio data in (ADC) |
| GP10 | GPIO | BYPASS | Preamp true bypass output _(active low)_ |
| GP11 | _Unused_ | | |
| GP12 | GPIO | BTN0 | Left footswitch button input |
| GP13 | GPIO | BTN1 | Right footswitch button input |
| GP14 | GPIO | SW0 | Left toggle switch input |
| GP15 | GPIO | SW1 | Right toggle switch input |
| GP16 | PWM | LED0 | Primary led indicator output |
| GP17 | PWM | LED1 | Secondary led indicator output |
| GP18 | _Unused_ | | |
| GP19 | _Unused_ | | |
| GP20 | I2C | SDA1 | Codec control data input/output |
| GP21 | I2C | SCL1 | Codec control clock |
| GP22 | GPIO | MUX | ADC multiplexer bank switch output _(active high)_ |
| GP26 | ADC | ADC0 | Input for POT0/3 |
| GP27 | ADC | ADC1 | Input for POT1/4 |
| GP28 | ADC | ADC2 | Input for POT2/5 |
