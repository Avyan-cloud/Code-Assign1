# Code-Assign1
from machine import Pin 
from time import sleep

# Odd-pos LED's
led1 = Pin(1, Pin.OUT)
led2 = Pin(2, Pin.OUT)
led3 = Pin(3, Pin.OUT)
led4 = Pin(4, Pin.OUT)
led5 = Pin(5, Pin.OUT)
led6 = Pin(6, Pin.OUT)
led7 = Pin(7, Pin.OUT)
led8 = Pin(8, Pin.OUT)

while True:
  for i in range(1, 9, 1):
    led = (i, Pin.OUT)
    led.value(1)
    sleep(0.5)

  for i in range(8, 0, -1):
    led = (i, Pin.OUT)
    led.value(0)
    sleep(0.5)
  
