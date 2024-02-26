## Build EXE for each measurement
1. Open the measurement lvproj for which you would like to build EXE, and select 'Build Specifications'.
    
    ![alt text](images/meas-lvproj.png)

2. Right click the build spec for UI packed library and click 'Build.

    ![alt text](images/build-ui-packed-lib.png)

3. Right click the build spec for Measurement EXE and click 'build'.
    
    ![alt text](images/build-measurement-exe.png)

4. Once the builds are complete, you should be able to see measurement EXE under /build folder.
    
    ![alt text](images/build-folder.png)

5. Under the measurement folder, you should able to see the EXE files.
    
    ![alt text](images/meas-exe-folder.png)

6. Parallel to the EXE, you should be able to see the UI packed library.
    
    ![alt text](images/meas-ui-folder.png)

7. Similarly, build EXEs for all the measurements.
    
    ![alt text](images/build-folder-with-all-meas.png)


Note: Please note that the /build folder must not be committed to repo and will be ignored by .gitignore upon commit.


## Build NIPKG for the plugin

1. Open the NIPM package build spec under /packages folder
    
    ![alt text](images/packages-folder.png)

2. Select the 'Audio ADC Measurements' Package under Packages tab. Ensure the version and other configurations are updated under Properties tab.
    
    ![alt text](images/nipb-package-properties.png)

3. In the Inputs tab, ensure the build folder is loaded with all measurement EXEs.
    
    ![alt text](images/nipb-inputs-tab.png)

4. Ensure the destination for the package installation is set to the below location:
    "C:\ProgramData\National Instruments\MeasurementLink\Services"

    ![alt text](images/nipb-destinations.png)

5. Click on 'Build Solution'.

    ![alt text](images/nipb-build-solution.png)

6. Once the build process is complete, you should be able to see a new version of package created in Packages folder parallel to build spec.
    
    Packages Folder:
   
    ![alt text](images/built-packages.png)

    Package File:
   
    ![alt text](images/nipm-package-file.png)


Note: Please note that the built NIPM packages must not be committed to repo. The folders created upon building NI PKG (Packages, ProcessingStage) will be ignored by .gitignore upon commit.


## Create and Update NIPM Feeds
1. The NIPM packages for different measurement plugins are added to an NIPM feed. So the users can install new packages or receive updates on existing feeds by subscribing to the feed.

2. The feeds for Measurement plugins are maintained under the below repo.
https://github.com/NI-MeasurementLink-Plug-Ins/package-manager-feeds

3. Please follow the procedure mentioned in below document for adding new packages or updating new versions of existing packages to the feed.
https://github.com/NI-MeasurementLink-Plug-Ins/package-manager-feeds/blob/main/package-feed-updater/README.md



