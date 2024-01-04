# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure
## ##Step1:
Use from robomaster import robot
## Step2:
Choose the x,y,z - axis movement
Step3:
Give ep_chassis.move to move straight
## Step4:
Give time.sleep() for a break
## Step5:
Give ep_chassis.drive_speed to have a circular movement



## Program
```python
from robomaster import robot
import time

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=2.5, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=255,effect="on")

    ep_chassis.move(x=0.5, y=0, z=85, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")
    
    ep_chassis.move(x=0.70, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=0,effect="on")

    ep_chassis.move(x=0.35, y=0, z=90, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=255,effect="on")

    ep_chassis.move(x=1.4, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=101,b=0,effect="on")
    
    ep_chassis.move(x=0, y=0, z=-40, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=1.63, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=0,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=143, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=51,b=102,effect="on")

    ep_chassis.move(x=0, y=1.55, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=51,b=102,effect="on")

    ep_chassis.move(x=2, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=128,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=82, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=0,b=225,effect="on")

    ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=204,b=225,effect="on")

    ep_chassis.move(x=0, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=225,effect="on")



    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()





    
    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

Insert image here

![IMG_20240102_141259](https://github.com/vigneshvickyu/mobilerobot-openloopcontrol/assets/151948835/297f0b19-eb27-4711-8e28-6af9e1f99ef2)
![WhatsApp Image 2024-01-04 at 16 37 06_423db6b7](https://github.com/vigneshvickyu/mobilerobot-openloopcontrol/assets/151948835/a5230b95-ed26-48d4-92af-054435f16dcf)
![WhatsApp Image 2024-01-04 at 16 39 28_ce76219d](https://github.com/vigneshvickyu/mobilerobot-openloopcontrol/assets/151948835/dbf9748a-4e4b-47ec-b978-ea7e41fdff07)
![image](https://github.com/vigneshvickyu/mobilerobot-openloopcontrol/assets/151948835/e4806d7a-f7fb-4e79-9c27-710e259181fc)


## MobileRobot Movement Video:
https://youtu.be/OHQbHIi6aLU?si=m33ulXRqN3ZMrBBi

Upload your video in Youtube and paste your video-id here


## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.



Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
