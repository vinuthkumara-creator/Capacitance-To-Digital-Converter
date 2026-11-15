# Applications
Applications
Why this circuit suits these uses

The circuit converts very small capacitance changes (pF range) into a voltage. Many physical quantities, such as water content, liquid level, and film thickness, change the capacitance of a pair of electrodes. This is mainly because water has a very high relative permittivity (about 80) compared with air (about 1) and dry soil (about 3 to 5). The design is fully analog, low cost, and low power, and it needs no microcontroller, so it suits remote or field sensing.

1. Soil moisture sensing

Two electrodes inserted in soil form a capacitor, with the soil as its dielectric. As moisture increases, the soil permittivity rises and so does the measured capacitance.

Use: irrigation control, precision agriculture, greenhouse monitoring, landslide and slope monitoring
Why it fits: moisture changes cause small capacitance shifts, which this pF-range circuit can resolve
Considerations: soil type, salinity, temperature, and electrode contact all affect readings, so per-soil calibration is needed
2. Rain and surface water flow measurement

Capacitive sensing can measure water level in a channel, gutter, or rain-gauge collection tube. Flow is then estimated from level using the known geometry of a weir, flume, or tipping bucket.

Use: rainfall monitoring, drainage and stormwater channels, flood warning systems
Why it fits: there are no moving parts to wear or clog, and a low-power analog front end can run for long periods outdoors
Considerations: the sensor measures level or water presence, so flow is calculated rather than measured directly
3. Cooling tower free-flow monitoring

In a cooling tower, water flows over the fill material and collects in the basin. Capacitive electrodes placed in the distribution basin, weir, or basin level can detect changes in water level or film presence. Changes in that signal can indicate variations in free flow, such as blocked nozzles, uneven distribution, or low flow.

Use: detecting flow variations and abnormal distribution, supporting maintenance and efficiency checks
Why it fits: non-intrusive sensing with no obstruction to the flow, and variations show up as capacitance changes
Considerations: humidity, temperature swings, scale and fouling on the electrodes, and water conductivity all affect readings. Insulated, protected electrodes and shielding help keep the signal stable
Other possible uses
Liquid level sensing in tanks
Humidity and leak detection
Proximity and displacement sensing
Limitations to mention
The sensor responds to capacitance, so flow and moisture are inferred and need calibration against a reference.
Stray capacitance becomes significant at pF levels, so shielding and a fixed layout matter.
Your measurements (3, 5 and 10 pF) show a response that isn’t perfectly linear, so a calibration curve should be used rather than a single linear conversion.
