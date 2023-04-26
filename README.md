# Sunsynk inverter Esphome

# Hardware:

1. RS485 Module (TTL -> RS485)
(https://www.robotics.org.za/RS485-MOD)

![image](https://user-images.githubusercontent.com/13587376/234514455-68eb6244-1da5-4967-82cd-034c172a47ba.png)

2. Any ESP module really
I used DF Robot Beetle ESP32 C3 - RISC-V
(https://robotics.org.za/DFR0868)

3. Connect:


    | RS485 side  | ESP32 side
      
    |DI -->       | ESP TX
    |DE & RE -->  | Control pin
    |RO -->       | RX

    | GND -->     | GND (ESP32)
    | VCC  -->    | VIN (ESP32) 5V

Attention:
Remove R7 on the RS485 module. otherwise the readings will be very sporadic


Power flow:
To show the power flow on your dashboard, add the power-flow in the Picture Elements Card Configuration file

![image](https://user-images.githubusercontent.com/13587376/234494799-3d959009-b19e-4531-91f8-28980415a05d.png)


# System mode:

On the dashboard add a Picture Elements Card Configuration - and add the details in the Picture Elements Card Configuration file

<img width="413" alt="image" src="https://user-images.githubusercontent.com/13587376/234494961-01776480-d7e5-43bf-9c42-c9559723bcad.png">
<img width="475" alt="image" src="https://user-images.githubusercontent.com/13587376/234502899-172496b2-a76c-4f2b-9373-f192cdb08742.png">
