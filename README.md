# DRV8870 Motor Controller

The Motor Controller, powered by Texas Instruments' DRV8870 motor drive, is a robust and efficient solution for running small to medium-sized DC motors. This compact device offers a 3.6V to 18V operating supply voltage range, ensuring compatibility with various power sources. It can efficiently drive a peak current of up to 3.6A, facilitating smooth motor operations even under demanding conditions. Equipped with advanced safety features like overcurrent, thermal, and undervoltage protection, the motor controller ensures your motor's longevity and reliable performance. Whether you're building a robot, an automatic door, or a smart home gadget, this motor controller offers easy integration and optimal performance, bringing your projects to life with precision and power.

## Features

 - PWM control
 - Motor Voltage 6.5V to 45V
 - Logic voltage 3.3V
 - Peak Current 3.6-A
 - 565mΩ Typical RDS(on) (high + low)
 - Dimensions 27 mm x 40 mm
 - Mounting hole diameter 3.2 mm
 - Low-Power Sleep Mode
 - Integrated Current Regulation
 - Overcurrent Protection
 - Thermal Shutdown
 - Automatic Fault Recovery
 - VM Undervoltage Lockout

## Examples

Here are example Arduino sketches that demonstrate how to control a DC motor using the DRV8870 Motor Controller

### PWM Control

```Arduino
// define the motor control pins
int in1Pin = 2;
int in2Pin = 3;

void setup() {
// set the motor control pins as outputs
pinMode(in1Pin, OUTPUT);
pinMode(in2Pin, OUTPUT);

// set the motor speed to half of the maximum
int speed = 127;

// set the direction to forward
digitalWrite(in1Pin, HIGH);
digitalWrite(in2Pin, LOW);

// apply the PWM signal to the EN pin
analogWrite(enPin, speed);
}

void loop() {
// do nothing
}
```

## Resources

- [DRV8870 Datasheet](https://www.ti.com/lit/ds/symlink/drv8870.pdf?ts=1688501994593&ref_url=https%253A%252F%252Fwww.ti.com%252Fproduct%252FDRV8870)