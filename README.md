# Capacitance-To-Digital-Converter
This project implements a reconfigurable analog circuit for measuring capacitance in the nanofarad (nF) and picofarad (pF) ranges. It is inspired by the capacitance-to-time converter (CTC) approach used for differential-type capacitive sensors (DCS), where the output is proportional to the capacitance change (ΔC).

# Reconfigurable Nano/Pico-Range Capacitance Measurement Circuit
 
A fully analog, reconfigurable circuit for measuring capacitance in the **nanofarad (nF)** and **picofarad (pF)** ranges, designed and simulated in **LTspice**.

```
ΔV proportional to [delta(C) x V] / Cs
```
 
where `Cs` is a known reference capacitor
 
## Block Diagram
 
```
Reference/Bias -> Signal Generation -> Conditioning/Filtering -> Buffer -> Rectifier/Detector -> Output
   (TL081)           (TL071)               (TL071, RC)          (TL071)      (D1, D2, TL071)      (DC)
```
 
> Replace with your own diagram image: `![Block diagram](images/block_diagram.png)`
 
## Circuit Description
 
| Stage | Op-amp | Function |
|-------|--------|----------|
| Reference / bias | TL081 | Resistive divider (R2 = 10 kΩ, R3 = 4.7 kΩ) sets the reference level |
| Signal generation | LM741 (U1) | Op-amp with R1 = 10 kΩ and C1 = 0.1 µF generates the excitation signal |
| Conditioning | LM741 (U2) | RC network (C2 = 50 nF, C3 = 47 nF, R4 = 100 kΩ) shapes the signal |
| Coupling / buffer | LM741 (U4) | C4 = 10 µF and R5 = 1 kΩ block DC and feed the next stage |
| Rectifier / detector | D1, D2, LM741 (U5) | Diodes with C5 = 10 µF and R6 = 100 kΩ convert the signal to a DC level proportional to capacitance |
 
 
## Repository Structure
 
```
.
├── circuit.asc        # LTspice schematic
├── images/            # Schematic and waveform screenshots
└── README.md
```
 
## Features
 
- Reconfigurable nF and pF measurement ranges
- Fully analog, no microcontroller needed
- Low-cost, built from standard op-amps (LM741, TL081)
- Output voltage proportional to measured capacitance

## Reference
Inspired by an IEEE Research based publication.
N. P. P. and S. Vijayakumar, "A Novel Capacitance-to-Time Converter for Differential-Type Capacitive Sensor Insensitive to Offset Mismatch and Parasitic Capacitance," in IEEE Sensors Letters, vol. 7, no. 10, pp. 1-4, Oct. 2023, Art no. 5502904, doi: 10.1109/LSENS.2023.3307069.
keywords: {Capacitance;Sensors;Capacitors;Capacitance measurement;Capacitive sensors;Prototypes;Manufacturing;Sensor systems;automatic offset-mismatch nullification (AOFN);capacitance-to-time converter (CTC);differential-type capacitive sensor (DCS)},

<img width="1062" height="832" alt="image" src="https://github.com/user-attachments/assets/ed8873a8-3ee3-4e37-9a6a-a259f5ac226b" />
