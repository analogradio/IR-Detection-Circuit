# IR-Detection-Circuit
optical heart rate sensor system (ECE 20008 SP'22)

For the optical sensor, we used an LED and a phototransistor. We used the IR204 and
PT204-6B since they have similar wavelengths. RD was chosen based on the maxim
forward current at the lowest forward voltage, so we picked RD = 100 ohms. RE was
chosen experimentally to be 2.2k ohms.

For the bandpass filter, we cascaded two active filters; a high pass filter and a low pass
filter, in order to only allow frequency only in the given range to pass through and impede
all the others. The high-pass filter filters the low frequencies, so its cutoff frequency will
be related to 40 BPM. The low-pass filter filters the high frequencies, so its cutoff frequency will be related to 200 BPM. Additionally, we chose the LM324N for the operational amplifiers.

For the comparator, we used the LM339 quad comparator to convert an analog signal to a digital output, that will turn on or off the red LED depending on the
output state.



