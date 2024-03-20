# AC
This service performs AC measurements: SNR, THD, THD+N, SFDR, Dynamic Range, Gain Error.

## Tested Hardware Setup 1

  ![alt text](meas-images/hardware-setup-for-CDB5381.png)

## Tested Hardware Setup 2

  ![alt text](meas-images/hardware-setup-for-TLV320ADC3101-K.png)

## InstrumentStudio Panel

### Usage

1. Select appropriate resource names, data line and channel according to the hardware setup and update other parameters as needed. Ensure the protocol settings are good. Please note that, measurement is working in I2S by default.

   ![alt text](meas-images/ac-config.png)

2. Run the measurement. The frequency, amplitude, SNR, THD, THD+N, Dynamic Range, Gain error, SFDR values are calculated and displayed in the panel below.

   ![alt text](meas-images/ac-meas-results.png)
3. The generated and acquired signals can be seen from time domain and frequency domain graphs.

   AC Measurement - Frequency Domain:
   ![alt text](meas-images/ac-freq-domain.png)

   AC Measurement - Time Domain:
   ![alt text](meas-images/ac-time-domain.png)



