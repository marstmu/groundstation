import serial

ser = serial.Serial('/dev/serial0', baudrate=9600)

current_message = ""

while True:
    data = ser.read().decode("utf-8", errors='ignore')
    if data == '\n':
        print(current_message)
        current_message = ""
    else:
        current_message += data
