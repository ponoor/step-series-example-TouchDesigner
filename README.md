# Step-series-example-TouchDesigner
This is a sample network for TouchDesigner to control the stepper driver STEP400 (and STEP800) over OSC. Please note that this sample controls only a single stepper motor.

## Covered commands
Currently only some basic commands are implemented to this sample. Although these commands are probably enough for many cases, the STEP400 has more commands for detailed control and status report. Alternatively there is a [sample Max patch](https://github.com/ponoor/step-series-example-Max) covering almost all functions of the STEP400.
Also please refer [the documentation](https://ponoor.com/en/docs/step400/osc-command-reference/) for further assistance.
Commands covered in this sample are:
- /setDestIp
- /setVoltageMode /setCurrentMode
- /run /goTo
- /setSpeedProfile
- /softStop /hardStop /softHiZ /hardHiZ
- /setServoMode /setTargetPosition
- /homing /getPosition

## Setting up
- Please refer the [Tutrial section of the STEP400](https://ponoor.com/en/docs/step400/tutorial/) for wiring and network configuration.
Be aware for the network address. This sample assumes that you hve configured the STEP400 to 10.0.0.101 and your PC to 10.0.0.10. In case you have different IP, please change them accordingly.
- Click "Activate" button to start OSC.
- Select motor ID where you connected the stepper motor.
- Select "Voltage" or "Current" mode. By clicking the slider, you can set the KVAL.
- Click "setDestIp" to set the destination where the controller needs to report to (your PC).
- Play around!

## Log
- First sample by [@loveandsheep](https://github.com/loveandsheep)
- 20210428 Added servo mode and homing. Updated by Yuske

## TouchDesigner Version
2021.12380
