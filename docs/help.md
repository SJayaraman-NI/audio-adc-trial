# Getting Started

## Adding a measurement panel to InstrumentStudio

1. Open InstrumentStudio
   ![alt text](images/instr-studio-open-is.png)

2. Click Manual Layout, and select required measurement under the collection (for e.g., AC under Audio ADC) and 'Create Large Panel' from dropdown. Click OK.
   ![alt text](images/instr-studio-manual-layout.png)

3. AC measurement UI will get displayed on a large panel as shown in below screenshot.
   ![alt text](images/instr-studio-ac-panel.png)


### Powering ON
Before starting the measurements, ensure the DUT is powered up. In case, SMUs are required to power up the DUT, add separate panel for configuring SMU voltages & other settings.

1. In a new Manual Layout, select required SMUs, Create Large Panel and click OK.

   ![alt text](images/instr-studio-smu-selection.png)

2. Set 12V and 5V Supplies according to the actual board connections: 

   Turn on the Output for each SMU and click Run. 
   
   ![alt text](images/instr-studio-smu-panel-1.png)

   ![alt text](images/instr-studio-smu-panel-2.png)

### Protocol configuration

1. In any measurement panel, click on three dots icon beside the Protocol settings header. Dialog box will be launched with I2S as default.
   Select the protocol which is required. It will automatically update the defaults of the settings.

   ![alt text](images/protocol-window.png)

2. Update any changes required in the settings of the selected protocol.
   
   ![alt text](images/protocol-window.png)

3. Click on close and settings will be updated in measurements.
   
   ![alt text](images/close-window.png)

## Adding a measurment step to TestStand 

Follow the worflow below to automate the measurements using TestStand and monitor it from Instrument Studio.

After adding measurement service into the Instrument Studio as explained above,

1. Open TestStand 2023 Q3 or higher version. Open a new sequence file and save the file. 

   ![alt text](images/teststand-open-seq.png)

2. Insert a 'Measurement' step under MeasurementLink in Insertion palette or by selecting Insert Step > MeasurementLink > Measurement in right click menu.
   Rename the step as required and choose the required measurement in Step settings.

   ![alt text](images/teststand-insert-measlink-step.png)

3. To transfer the measurement configuration from the Instrument Studio to the TestStand, click on "COPY button" highlighted in the screenshot.

   ![alt text](images/instr-studio-copy-meas-config.png)

4. The below indication confirms the Measurement configuration is copied

   ![alt text](images/instr-studio-meas-config-copied.png)

5. Select the measurement step and click on the paste button as highlighted in the screenshot. There will be a message indicating that the measurement configuration is applied.

   ![alt text](images/teststand-paste-config.png)

6. Set 'Enable Monitoring' variable to True as shown in below screenshot. It will help us to monitor the results in Instr Studio.

   ![alt text](images/teststand-enable-monitoring.png)

8. Save the Sequence file and RUN the sequence. While running the sequence file in TestStand you can see measurement results and graphs updated in the InstrumentStudio as well.

   ![alt text](images/teststand-run-seq.png)

9. The measurement results are updated in the Instrument Studio as below.

   ![alt text](images/instr-studio-results-from-ts.png)

Please refer [this](measurements\meas-index.md) for more details on each measurement.