# Different-function-of-pi-camera-using-respberry-pi


import RPi.GPIO as GPIO
from time import sleep
GPIO.setwarnings(False)
GPIO.setmode(GPIO.BOARD)
#BCM

GPIO.setup(8, GPIO.OUT, initial = GPIO.LOW)
GPIO.setup(10, GPIO.OUT, initial = GPIO.LOW)
GPIO.setup(12, GPIO.OUT, initial = GPIO.LOW)

while (True) :
    print("High")
    GPIO.output(8, GPIO.HIGH)
    sleep(1) # In Seconds
    print("LOW")
    GPIO.output(8, GPIO.LOW)
    sleep(1)
    print("High")
    GPIO.output(10, GPIO.HIGH)
    sleep(2) # In Seconds
    print("LOW")
    GPIO.output(10, GPIO.LOW)
    sleep(1)
    print("High")
    GPIO.output(12, GPIO.HIGH)
    sleep(3) # In Seconds
    print("LOW")
    GPIO.output(12, GPIO.LOW)
    sleep(1)
