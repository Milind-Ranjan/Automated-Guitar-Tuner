## Arduino Automatic Guitar Tuner

**README.md**

This repository contains the code for an Arduino-based automatic guitar tuner. It utilizes a stepper motor to adjust the tuning based on the detected frequency of the string.

### Features

* Selects a string for tuning (E2 to E4)
* Records audio from the guitar string
* Performs Fast Fourier Transform (FFT) to analyze frequency
* Calculates the difference between measured and target frequency
* Adjusts the stepper motor to achieve the desired tuning
* Provides feedback on the measured frequency, target frequency, and adjustment steps

### Hardware Requirements

* Arduino board (any model with enough pins)
* Stepper motor (including driver shield if necessary)
* Microphone (piezoelectric or electret)
* Connecting wires
* Guitar

### Software Requirements

* Arduino IDE ([https://www.arduino.cc/](https://www.arduino.cc/))
* Libraries:
    * arduinoFFT
    * AccelStepper

**Note:** You may need to install the libraries mentioned above through the Arduino IDE Library Manager.

### Using the Code

1. **Download or clone this repository.**
2. **Install the required libraries in your Arduino IDE.** You can find them in the Library Manager by going to Sketch > Include Library > Manage Libraries. Search for the library names and install them.
3. **Connect the hardware components according to the pin definitions in the code (`guitar_tuner.ino`).** The code should have comments specifying which pins connect to each component.
4. **Open `guitar_tuner.ino` in the Arduino IDE.**
5. **Upload the code to your Arduino board.**
6. **Follow the on-screen instructions to select a string and initiate tuning.**

### Additional Information

* The code assumes a reference pitch of A4 = 440 Hz. You can modify this value in the code if needed.
* The calibration of the stepper motor for tuning adjustments might require fine-tuning based on your specific setup. This may involve adjusting values in the code related to the stepper motor steps and frequency conversion.

### Contributing

We welcome contributions to improve this project. Feel free to fork the repository, make changes, and submit a pull request.
