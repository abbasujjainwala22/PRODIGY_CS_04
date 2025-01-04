# KEYSTROKE LOGGER
Python Code which can be used to spy on different systems as it gives as the exact keys pressed on keyboard

# Description

This Python script is a simple keystroke logger. It uses the 'keyboard' library to detect and record every key press on your keyboard. The recorded keystrokes are then saved into a text file named 'keystrokes.txt'.

# Code Structure

The script is structured as follows:

1. Importing the library: The 'keyboard' library is imported which provides the functionality to monitor keyboard inputs.
2. File name definition: The 'log_file' variable is defined to store the name of the file where the keystrokes will be logged.
3. Function definition: The 'on_key_press(event)' function is defined. This function is triggered every time a key is pressed. It opens the log file in append mode and writes the name of the key pressed into the file.
4. Event hook: The 'keyboard.on_press(on_key_press)' line sets up the event hook, telling the 'keyboard' library to call our 'on_key_press' function every time a key is pressed.
5. Wait: The 'keyboard.wait()' line causes the script to run indefinitely, waiting for key press events.

# Usage

To use this script, you need to have Python and the `keyboard` library installed on your machine. If you don't have the 'keyboard' library, you can install it using pip:

pip install keyboard

After installing the necessary prerequisites, you can run the script using Python:

python keystroke_logger.py

Please replace 'keystroke_logger.py' with the name of your python file.

# Example

After running the script, every key you press will be logged into 'keystrokes.txt'. For example, if you press 'a', 'b', and 'c', you'll find the following in 'keystrokes.txt':

a
b
1
enter
space

# Disclaimer

Please note that this script is provided for educational purposes only. Unauthorized keylogging is illegal and unethical. Always obtain proper authorization before monitoring keyboard inputs.
