# Voice-Controlled 7-Segment Display

This project integrates Python-based voice recognition with Arduino to control a 7-segment display. Users can speak numbers (0-9), which are recognized by the Python script and displayed in real time on the 7-segment display.

## Features
- **Voice Recognition:** Processes spoken input to identify numbers using Python.
- **Arduino Control:** Communicates with the 7-segment display to visualize the recognized number.
- **Real-Time Operation:** Seamlessly bridges software and hardware for instant feedback.

## Technologies Used
- **Python:** For voice recognition and processing.
- **Arduino:** For controlling the 7-segment display.
- **Serial Communication:** Ensures smooth data transfer between Python and Arduino.

## How to Run

### Prerequisites
1. Install Python (3.8 or higher).
2. Install the necessary Python libraries:
   ```bash
   pip install speechrecognition pyserial
   ```
3. Set up the Arduino IDE on your computer.
4. Connect the 7-segment display to the Arduino as per the wiring diagram.
5. Upload the Arduino code to the microcontroller.

### Steps
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/voice-controlled-7seg.git
   cd voice-controlled-7seg
   ```

2. **Prepare the Arduino:**
   - Open the `arduino_code.ino` file in the Arduino IDE.
   - Verify and upload the code to your Arduino board.

3. **Run the Python Script:**
   - Ensure the Arduino is connected to your computer via USB.
   - Locate the COM port used by the Arduino (e.g., COM3 on Windows or `/dev/ttyUSB0` on Linux/Mac).
   - Modify the `python_script.py` to set the correct COM port if needed.
   - Execute the script:
     ```bash
     python python_script.py
     ```

4. **Speak a Number:**
   - The Python script will prompt you to speak.
   - Say any number between 0 and 9.
   - The number will be displayed on the 7-segment display in real time.

### Additional Instructions
This is a program that recognizes speech from numbers 1 to 9 and displays them on the seven-segment display using Arduino.

#### Steps to Follow
1. Use the `.png` image file to draw the circuit of the Arduino.
2. Upload the `.ino` file using Arduino IDE to your Arduino Uno.
3. Open the `.py` file and run the code. Say the number you want to display.

**Note:**
- You might need to install the following packages on your CMD:
  ```bash
  pip install pyserial
  pip install SpeechRecognition
  ```
- The `speech_recognition` library uses Google AI, so an active internet connection is required.

### Notes
- Ensure a quiet environment for better voice recognition accuracy.
- Double-check the wiring for the 7-segment display to avoid errors.

## Future Improvements
- Add support for additional commands.
- Expand functionality to display multi-digit numbers.
- Integrate advanced voice processing for improved recognition.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---
Feel free to contribute to the project or report issues via GitHub!
