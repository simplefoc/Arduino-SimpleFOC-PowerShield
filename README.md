# Arduino *Simple**FOC** PowerShield* *v0.3 ( in testing - problems encountered)* 
A powerful arduino shield for running BLDC motors using the FOC algorithm. This board is based on the [BTN8982](https://www.infineon.com/dgdl/Infineon-BTN8982TA-DS-v01_00-EN.pdf?fileId=db3a30433fa9412f013fbe32289b7c17) half bridges and can support currents up to 30 Amps continuos and 50Amps peak. Making it a board that can run virtually any BLDC motor.

> *Simple**FOC** PowerShield* *v0.3* is still in testing and it is not released yet. It is possible that some changes will be included in the official release. If you are interested in fabricating your-own ***Power**Shield* please check the earlier [releases](https://github.com/simplefoc/Arduino-SimpleFOC-PowerShield/releases)!

<p align="">
<img src="./images/top.png"  height="320px"><img src="./images/bottom.png"  height="320px">
</p>

### Features
- **Plug & play**: In combination with Arduino *Simple**FOC**library* - [github](https://github.com/simplefoc/Arduino-FOC)
- **Low-cost**: Price of €25-€35 -  **Will be available soon in the [shop](https://simplefoc.com/shop)! (est. June 2021)**
- **In-line current sensing**: - measuring up to 33Amps bidirectional
- **Max power >500W**: max current 30A, power-supply up to 35V
- **Arduino headers**: Arduino UNO, Arduino MEGA, STM32 Nucleo boards, Aruidno DUE...
- **Small size**: 53mm x 61mm
- **Stackable**: running 2 motors in the same time
- **Configurable pinout**: Hardware configuration - soldering connections
- **Encoder/Hall sensors interface**: Integrated 3.3kΩ pullups (configurable)
- **I2C interface**: Integrated 4.7kΩ pullups (configurable)
- **Open Source**: 
   - Fully available fabrication files  
        - If never done it before, see a similar guide for *Simple**FOC**Shueld*:  [how to make it yourself](https://docs.simplefoc.com/arduino_simplefoc_shield_fabrication)
   - Altium project
   - 3d model
   - schematics
