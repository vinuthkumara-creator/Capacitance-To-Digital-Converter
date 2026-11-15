# Experimental Results: Pico-Range Capacitance Measurements

This section shows oscilloscope captures of the circuit measuring known capacitors in the **pF range**. Each capture shows the circuit output for a different capacitance under test (Cx).

## Test Setup

<img width="967" height="733" alt="image" src="https://github.com/user-attachments/assets/08e41b6b-c2e9-4439-ac6a-404f4252e496" />


- **Circuit:** Reconfigurable capacitance measurement circuit (see main `README.md`)
- **Capacitors under test:** 3 pF, 5 pF, 10 pF
- **Supply:** ±5 V
- **Reference capacitor (Cref):** 10 pF
- **Instrument:** _TODO: oscilloscope model_
- **Probe settings:** _TODO: e.g. 1x / 10x, time/div, volts/div_

## Measurements

### 3 pF

- **Capacitance under test:** 3 pF

<img width="881" height="695" alt="WhatsApp Image 2026-11-1" src="https://github.com/user-attachments/assets/d0a87296-add6-4b0b-be85-989ef4d7b638" />


### 5 pF

- **Capacitance under test:** 5 pF

<img width="662" height="532" alt="image" src="https://github.com/user-attachments/assets/f4f7b4a9-a2db-4d88-bb44-8bdf249a125a" />


### 10 pF

- **Capacitance under test:** 10 pF

<img width="642" height="487" alt="image" src="https://github.com/user-attachments/assets/e0b9c062-fff9-4dde-ae71-23b5193dff08" />


## Summary

| Capacitance (pF) | Measured output (V) | Notes |
|------------------|---------------------|-------|
| 3 | 1.23 | |
| 5 | 1.42 | |
| 10 | 2.46 | |

<img width="1600" height="1000" alt="image" src="https://github.com/user-attachments/assets/24ae4fa2-10dc-4fd9-8704-bc81983b9020" />

Approximately a linear response can be observed. The same results can be observed even for nF or uF range, the requirement is that we have to reconfigure a suitable value for the reference capacitor. 
