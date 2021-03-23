# Password-based-Security-Door-Lock-System-

- Discription : 
Password based Security Door Lock based on 2 ATmega16 microcontrollers, the first is
“HMI” for user interface, and the second is a ‘controller’ which is responsible for the system 
operations and control. 
 
- Detailed Process:
The user should enter the desired password 2 times in the beginning. If the entered passwords are matched, the UART send the password to the EEPROM attached to the second microcontroller and will be saved permanently .If not, the user shall repeat the operation of entering the new password. 

After the desired password is saved successfully ,the user have the option to select between changing the current password with new one or opening the door .By selecting the first option ,he will be asked to enter the current password then enter the new password 2 times to be saves in the EEPROM. But if the user select the second option, the current password will be asked to rotate the door clockwise for 15 sec and the same in the reverse direction.
A led will be on as a simulation of a buzzer if the password entered wrong 3 times.


- Drivers designed and implemented for the project: Timer, Keypad, LCD, 
DC Motor, UART, I2C and External EEPROM.Drivers are implemented using configuration technique "Static and Dynamic" to support different modes in Atmega16.Different design methods are used like interrupts, call backs, tight and periodic polling.

- The file attached in the reposirty contains a well written and readable code with good comments and a Project simulation using Proteus design Program.
