# Arduino *Simple**FOC** PowerShield* *v0.2* 
A powerful arduino shield for running BLDC motors using the FOC algorithm. This board is based on the [BTN8982](https://www.infineon.com/dgdl/Infineon-BTN8982TA-DS-v01_00-EN.pdf?fileId=db3a30433fa9412f013fbe32289b7c17) half bridges and can support currents up to 30 Amps continuos and 50Amps peak. Making it a board that can run virtually any BLDC motor.

<p align="">
<img src="images/top.png"  height="320px"><img src="images/bottom.png"  height="320px">
</p>

### Features
- **Plug & play**: In combination with Arduino *Simple**FOC**library* - [github](https://github.com/simplefoc/Arduino-FOC)
- **Low-cost**: Fabrication price under €25/pcs - **will not be sold by silplefoc.com**
- **High-side current sensing**: - not yet supported by *Simple**FOC**library*
- **In-line current sensing**: - supported by *Simple**FOC**library*
- **Max power <500W**: max current 30A, power-supply 24V
- **Arduino headers**: Arduino UNO, Arduino MEGA, STM32 Nucleo boards, Aruidno DUE...
- **Small size**: 53mm x 60mm
- **Encoder/Hall sensors interface**: Integrated 3.3kΩ pullups (configurable)
- **Open Source**: 
   - Fully available fabrication files  
        - If never done it before, see a similar guide for *Simple**FOC**Shueld*:  [how to make it yourself](https://docs.simplefoc.com/arduino_simplefoc_shield_fabrication)
   - Altium project
   - 3d model
   - schematics
    
#### Future features
- **Stackable**: running 2 motors in the same time
- **I2C interface**: Integrated 4.7kΩ pullups (configurable)
- **Configurable pinout**: Hardware configuration - soldering connections

> New version of the *Simple**FOC** PowerShield* is in the development at the moment (*v0.3*).
> The first versions are currently in testing. For more info check the [developmental branch](https://github.com/simplefoc/Arduino-SimpleFOC-PowerShield/tree/dev) 

### Pinouts
At this point ***Power**Shield* has fixed pinout.

#### Driver pinout
Signal | Description | Pin number
--- | --- | ----
IN1 | pwm 1 |	9
IN2 |  pwm 2 |	6
IN3 | 	pwm 3	 | 5 
INH1| enable 1 |	8
INH2 |	enable 2 |	7
INH3 |	enable  3	| 4

#### Current sensing pinout
Signal | Description | Pin number
--- | --- | ----
CS1 | in-line current sense - phase 1/A| A0
CS2 | in-line current sense - phase 3/C | A1
IS1 | high-side current sense - phase 1/A | A2
IS2 | high-side current sense - phase 2/B | A3

#### Sensor input pinout
Signal | Description | Pin number
--- | --- | ----
A/ U | Encoder A, Hall sensor U |	10
B/ V | Encoder B, Hall sensor V |	11
I/ W | Encoder C, Hall sensor W |	12

<p align="">
<img src="images/small.jpg"  height="320px">
</p>
