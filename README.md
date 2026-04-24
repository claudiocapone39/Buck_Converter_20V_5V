# Synchronous Buck Converter 10-20V to 5V

This Synchronous Buck converter takes 10-20V range as input voltage and outputs 5A@5V. 
It features an LCD screen to show information and a user button to interact with the device.
The board features an LPC1313 NXP Microcontroller in addition with a buffer stage and RC filter for accurate feedback acquisition.

<img width=50% height=50% alt="Buck_Converter_PCB_isometric" src="https://github.com/user-attachments/assets/5d0bc755-0999-4f5c-b4dd-5cbbbefad3f8" />

  <img width="519" height="300" alt="Buck_Converter_Block_Schematic" src="https://github.com/user-attachments/assets/9c526122-3554-48aa-96f1-224c51d084e6" />

<br>

## SIMETRIX
  
  The converter has been simulated through the use of SIMETRIX software. 
  In this schematic, the PWM signals from the MCUs have been implemented as ideal pulse generators (INA and INB)
  
  <br>
  
  <img width="788" height="397" alt="Buck_Converter_Synchronous_20V_Simetrix" src="https://github.com/user-attachments/assets/091b51b1-ebef-44f8-afc2-9658dc0fa591" />

  <br>

  - UCC27282 is the Gate Driver of the MOSFETs RSS065N06HZG
  - LP38691 is the LDO that outputs 3.3V
  - OPA827 works both as a buffer for the voltage divider signal and as an RC filter

The output of the buck converter, after a short transient, gets stable at 5V.

<br>

<img width="326" height="410" alt="Buck_Converter_VOUT" src="https://github.com/user-attachments/assets/19201cad-ff93-49c0-824c-85baa80f5001" />

<br>

The output of the op-amp is the voltage reference for the MCU's ADC. After a short transient, it gets stable at 3.3V

<img width="330" height="397" alt="Buck_Converter_X1-OUT" src="https://github.com/user-attachments/assets/30aedaee-2057-4bf1-9722-7f1ebe6e5ba5" />

<br>

The converter's efficiency has been evaluated as the ratio between output and input power.

<br>

<img width=40% height=40% alt="Buck_Converter_Efficiency_report" src="https://github.com/user-attachments/assets/0c3d42b8-894c-422e-ac82-2e840931bb92" />

## PCB
The PCB has been designed in Autodesk Fusion 360


<img width=50% height=50% alt="Buck_Converter_PCB_top" src="https://github.com/user-attachments/assets/2bcdf24f-e6ad-4584-aee3-013117fbfdd6" />





