# -PLC-PID-LEVEL-CONTROL
**PID Level Control** is a PLC based industrial application for controlling the water level in a tank with a PID controller.Tia portal V15 has been used for the programing.
Factory i/o has been used for the 3D simulation. S7-PLCSIM has been used instead of a real PLC.

## Main Idea

From the `Electric Switchboard` next to the station you choose the desired setpoint with the help of a `potentiometer`. From there you can observe
from three displays the set point value, 
the value of the liquid in the tank every moment and the error(setpoint-liquid level).
Depends on the setpoint value a filling valve or discharge valve opens so the level of the liquid be equal to the setpoint.
A PID controller controlling the flow of the valves.
From the main `HMI screen` you can start the process, drain some of the liquid (or drain all the liquid) and an emergency stop switch is available.
You can also supervise the Ki, Kp, Kd values and the setpoint, error and liquid level values.
From the admin `HMI screen`(password protected) you can adjust the Ki, Kp, Kd values or stop the PID controller(but not the process).
An error `HMI screen` is also available to monitor for errors or warnings in the process(warning 1 :Ki has a big value , warning 2 :Kd has a value)

(log in information's for the admin screen is username: admin , Password:12345)




## Devices

- **PLC**:  `S7-1200`,

    **CPU**: `1211C DC/DC/DC`,

    **Description** : Work memory 50 KB; 24VDC power supply with DI6 x 24VDC SINK/ SOURCE, DQ4 x 24VDC and AI2 on
board;3 high-speed counters (expandable with digital signal board) and 4 pulse outputs on board; signal board expands on-board I/O; up to 3 communication modules for serial communication; 0.04 ms/1000 instructions; PROFINET interface for programming, HMI and PLC to PLC communication

- **HMI**: `TP700 Comfort`


## IMAGES

**FACTORY IO IMAGE**

![factoryioimg.jpg](/img/factoryioimg.jpg)

**HMI IMAGES**

![HMImain.jpg](/img/HMImain.jpg)
![HMIadmin.jpg](/img/HMImain.jpg)
![HMIerror.jpg](/img/HMIerror.jpg)


## Files
- **levelcontrolcode.pdf** : it's the plc code
- **LevelControlHMI.pdf** : it's the HMI settings
- **vids** : it's the file with demonstration of how it works `(video1MainHmi= video with the main screen on work)``(Admin&ErrorHmi= video with the admin and error screen on work)`
- **levelcontrol.factoryio**: it's the factory io file 
- **Filling Tank**: it's the folder for the tia portal

