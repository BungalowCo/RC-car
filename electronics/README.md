# E Section
The electronics of this project compromises of two sections, the RC Transceiver(Controller) and the RC Receiver(car electronics). The radio communication for the project is based on the NRF24L01 transceiver module and the micro-controller is an arduino pro mini.

## RC Arduino RC transmitter
The RC Arduino RC transmitter is a universal controller that was built following this [How To Mechatronics guide](https://howtomechatronics.com/projects/diy-arduino-rc-transmitter/). The radio communication of this controller is based on the NRF24L01 transceiver module which if used with an amplified antenna it can have a stable range of up to 700 meters in open space. It features 14 channels, 6 of which are analog inputs and 8 digital inputs. It has two joysticks, two potentiometers, two toggle switches, six buttons and additionally an internal measuring unit consisting of an accelerometer and a gyroscope which can be also used for controlling things with just moving around or tilting the controller.

### Arduino RC Transmitter Circuit Diagram
![image](https://user-images.githubusercontent.com/37361299/128600323-fe440f4e-94e6-4ddc-8a53-ccf22cd9071c.png)
### PCB Design
![Screen Shot 2021-08-07 at 10 38 00 pm](https://user-images.githubusercontent.com/37361299/128600369-490c64d5-1b14-4220-a2bd-fdd542859d77.png)
### Mock RC receiver
A mock RC receriver was used to tests the connection of the controller and its inputs.
![image](https://user-images.githubusercontent.com/37361299/128600442-4abea3b2-2a91-416b-851d-a86f11f7c1c7.png)

## Car electronics
The car electronics is separated into three sections: the RC receiver, motor and steering. The RC receiver consists of an Arduino pro mini and NRF24L01 transceiver module. For the motor, a 1000KV brushless motor is used with 30A ECS. The steering is done with a MG996R high-torque servo motor which is also connected to the ECS. The car electronics is powered by a 3S 11.1V 2800mAh 35C Lipo Batter using the ESC's Battery Eliminator Circuit feature to provide 5V to the receiver.
![image](https://user-images.githubusercontent.com/37361299/128601424-19d46e85-ba67-4810-896d-1d5eae15320d.png)
