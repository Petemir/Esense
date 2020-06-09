# Esense

This is an Android application. The app establishes connection with a Bluetooth Low Energy (BLE) earble device named [eSense](http://www.esense.io/). The device is developed by NOKIA Bell Labs Cambridge. <br/>
![](images/esensedevice.png)
<br/>The device contains sensor which provides accelerometer and gyroscope data. From this data hand and mouth related activities like eating, swallowing, speaking, head shaking etc. can be recognized by machine learning algorithms like CNN, LSTM.

# IDE

- **Android Studio**

# Architecture
- The eSense device gets connected with mobile via Bluetooth. Once the connection gets established, the sensor data is recorded.
![](images/architecture.png)

# Application Overview
- Clicking the **Connect** button user connects eSense device with mobile
- After selecting any **activity** , if user click **Start** icon the data will start to be recorded
- Clikcing the **Stop** icon will save the recorded data in mobile
- User can also see the recorded activity history
![](images/appoverview.png)

# Data Collection
From the earable device 3 types of data can be collected.
  - **Audio**
  - **Accelerometer**
  - **Gyroscope**

The accelerometer and gyroscope data is saved in mobile storage as **.csv** format. On the other hand audio data is saved as **.3gpp** format in mobile storage.
![](images/datatype.png)

# Add Ons
As an extension of the work by [Shafiqul Islam](https://github.com/shafiqulislamsumon/Esense) the app now allows recording data labeled as "Experiment". The exported data is marked with this label and a corresponding number which allows easy discrimination of recording states for further processing (i.e. "Experiment" vs "Walking" data). 
Additionally, a new button was created that labels data as collected during the "ON" vs "OFF" period. This functionality can be used to section different parts of one recording (i.e. one recording containing several smaller parts with transition periods).  
<img src="https://github.com/SabrinaFrohn/Esense/tree/master/images/app_with_onOff_experiment.png" alt="App screenshot" width="360" hight="640"/>
