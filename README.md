# Arduino *Simple**FOC** PowerShield* *v0.2* 
A powerful arduino shield for running BLDC motors using the FOC algorithm. This board is based on the [BTN8982](https://www.infineon.com/dgdl/Infineon-BTN8982TA-DS-v01_00-EN.pdf?fileId=db3a30433fa9412f013fbe32289b7c17) half bridges and can support currents up to 30 Amps continuous and 50Amps peak. Making it a board that can run virtually any BLDC motor.

<p align="">
<img src="images/top.png"  height="320px"><img src="images/bottom.png"  height="320px">
</p>


<blockquote class="warning"><p class="heading"> ⚠️ BEWARE: BTN8982/IFX007T performance issues</p><p>BTN8982 and IFX007T drivers have been designed for DC motors and are based on old H-bridge technology. They have very long mosfet rise time (multiple microseconds) which in many cases presents a considerable part of the PWM duty cycle. When running the BLDC motors, precise PWM duty cycle setting is crucial for smooth and efficient operation. Therefore these drivers will not be able to provide very smooth operation on high frequency PWM (above 15kHz). Read more about it in the community thread: <a href="https://community.simplefoc.com/t/simplefoc-powershield/582">link</a>.<br> This performance constraint is the main reason why the <span class="simple">Simple<span class="foc">FOC</span> <b>Power</b>Shield</span> project has for now been put on hold, and although these boards are available through Aliexpress and some other platforms, they will not be available through simplefoc.com. <br><br></p><p>This does not mean that the board itself is not functional or that it will not work in your project though. It is still one of the cheapest (simplest) solutions out there for mid to high power BLDC control and with proper tuning of control loops you will still be able to get some good results with it.</p></blockquote>


### Features
- **Plug & play**: In combination with Arduino *Simple**FOC**library* - [github](https://github.com/simplefoc/Arduino-FOC)
- **Low-cost**: Fabrication price under €25/pcs - **will not be sold by simplefoc.com**
- **High-side current sensing**: - not yet supported by *Simple**FOC**library*
- **In-line current sensing**: - supported by *Simple**FOC**library*
- **Max power <500W**: max current 30A, power-supply 24V
- **Arduino headers**: Arduino UNO, Arduino MEGA, STM32 Nucleo boards, Aruidno DUE...
- **Small size**: 53mm x 60mm
- **Encoder/Hall sensors interface**: Integrated 3.3kΩ pullups (configurable)
- **Open Source**: 
   - Fully available fabrication files  
        - If never done it before, see a similar guide for *Simple**FOC**Shield*:  [how to make it yourself](https://docs.simplefoc.com/arduino_simplefoc_shield_fabrication)
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
