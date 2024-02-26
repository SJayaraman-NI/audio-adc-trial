# Getting Started

## Adding a measurement panel to InstrumentStudio

1. Open InstrumentStudio
   ![alt text](images/instr-studio-open-is.png)

2. Click Manual Layout, and select required measurement (e.g., Audio ADC - AC Measurement) and 'Create Large Panel' from dropdown. Click OK.
   ![alt text](images/instr-studio-manual-layout.png)

3. AC measurement UI will get displayed on a large panel as shown in below screenshot.
   ![alt text](images/instr-studio-ac-panel.png)


### Powering ON
1. In a new Manual Layout, select required SMUs, Create Large Panel and click OK.

   ![alt text](images/instr-studio-smu-selection.png)

2. Set 12V and 5V Supplies according to the actual board connections: 

   Turn on the Output for each SMU and click Run.
   ![alt text](images/instr-studio-smu-selection.png)

### Protocol configuration

1. In AC Measurement panel, click on three dots icon beside the Protocol settings header. Dialog box will be launched with I2S as default.
   Select the protocol which is required. It will automatically update the defaults of the settings.

   ![alt text](images/protocol-window.png)

2. If there are any changes in the settings of the selected protocol making changes in settings section.
   
   ![alt text](images/protocol-window.png)

3. Click on close and settings will be updated in measurements.
   
   ![alt text](images/close-window.png)

## Adding a measurment step to TestStand 

The following workflow provides an example to show how we can automate our measurements using TestStand from the Instrument Studio and also shows how monitoring can be done. 

After following above steps to add measurement service into the Instrument Studio.

1. Open TestStand 2023 Q3 or higher version. Open new sequence file or saved sequence file. 

   ![alt text](images/teststand-open-seq.png)

2. Insert a 'Measurement' step under MeasurementLink in Insertion palette or by selecting Insert Step > MeasurementLink > Measurement in right click menu.

   ![alt text](images/teststand-insert-measlink-step.png)

3. To transfer the measurement configuration from the Instrument Studio to the TestStand, click on "COPY button" highlighted in the screenshot.

   ![alt text](images/instr-studio-copy-meas-config.png)

4. The below indication confirms the Measurement configuration is copied

   ![alt text](images/instr-studio-meas-config-copied.png)

5. Select the measurement step click on the paste button as highlighted in the screenshot. There will be message indicating that the measurement configuration is applied.

  ![alt text](images/teststand-paste-config.png)

6. Save the Sequence file and RUN the sequence. While running the sequence file in TestStand you can see measurement resultant graphs and results  updated in the InstrumentStudio as well.

   ![alt text](images/teststand-run-seq.png)

7. The measurement results are updated in the Instrument Studio as below.

   ![alt text](images/instr-studio-results-from-ts.png)

## Measurements
### AC

1. Select appropriate resource names, data line and channel according to the hardware setup and DUT specs. Ensure the protocol settings are good. Please note that, measurement is working in I2S by default.

   ![alt text](images/ac-config.png)

2. Run the measurement. The frequency, amplitude, SNR, THD, THD+N, Dynamic Range, Gain error, SFDR values are calculated and displayed in the panel below.

   ![alt text](images/ac-meas-results.png)
3. The generated and acquired signals can be seen from time domain and frequency domain graphs.

   AC Measurement - Frequency Domain:
   ![alt text](images/ac-freq-domain.png)

   AC Measurement - Time Domain:
   ![alt text](images/ac-time-domain.png)

### Frequency Response

1. Select the appropriate resource names, data line, channel the DUT is connected to and run the measurement service with the default values.
   ![alt text](images/freq-resp-config.png)

2. FR, RMS Levels, THD, THD+N, time domain graphs should be visible without any error.

   Frequency Response:
   ![alt text](images/freq-resp-FR.png)

   RMS Levels:
   ![alt text](images/freq-resp-rms-levels.png)

   THD:
   ![alt text](images/freq-resp-thd.png)

   THD+N:
   ![alt text](images/freq-resp-thd-plus-n.png)

   TimeDomain:
   ![alt text](images/freq-resp-time-domain.png)
