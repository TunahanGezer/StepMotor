# Stepper Motor Driver with STSPIN820

This project is a **Stepper Motor Driver** system using the **STSPIN820** IC, which allows for precise motor control with adjustable TOFF timing and micro-stepping modes. The system can be used for various stepper motor applications requiring precision and control.

## Components Used

- **STSPIN820 Stepper Motor Driver**
- **Stepper Motor** (Bipolar/Unipolar)
- **Microcontroller** (ESP32, Arduino, etc.)
- **2x 8-pin Headers** (for motor and signal connections)
- **Power Supply** (12V or 24V, depending on the motor)
- **Resistors** (for current sensing on SNS A and SNS B)
- **Breadboard** and **Jumper Wires**

## How It Works

1. The **STSPIN820** driver is connected to the stepper motor and the microcontroller.
2. The motor phases are monitored through **SNS A** and **SNS B** pins.
3. The **TOFF** pin is adjusted to set the motor's off-time, optimizing performance.
4. The microcontroller sends control signals to **EN/FAULT** and **StandBy** to activate the motor and monitor faults.
5. The **MODE** pin sets the micro-stepping mode, controlling the precision of motor movements.
6. The **REF** pin adjusts the motor’s current reference to control speed and torque.

## Project Files

- **Circuit Diagram**: [Link to schematic]
- **PCB Design**: [https://github.com/TunahanGezer/StepMotor/blob/main/PCB-step-motor.jpg]

## How to Use

1. Connect the **STSPIN820** driver to your stepper motor and microcontroller according to the schematic.
2. Upload the provided control code to your microcontroller.
3. Adjust the **TOFF** pin as needed for optimal motor performance.
4. Enable the motor using the **EN/FAULT** pin and set the stepping mode using the **MODE** pin.
5. Supply power to the **MOTOR VOLTAGE** pin (12V or 24V depending on the motor) and observe the motor operation.

## Future Improvements

- Add additional step modes for more precise control.
- Implement dynamic speed control based on sensor feedback.
- Integrate a user interface for manual or automated motor control.
