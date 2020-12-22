# gps-sensor-embedded
A program for handling data fetched from the adafruit! Ultimate GPS Breakout v3“ GPS sensor. Fetched data is displayed on a LCD screen connected to the ATMega16A microcontroller which is integrated in the 
Mega16mini developer kit. The microcontroller is used for powering the GPS module and for handling the data fetched from the module. 

# Hardware scheme
[![shema-hardvera.png](https://i.postimg.cc/6QvZP3F9/shema-hardvera.png)](https://postimg.cc/3y3W4KK6)

# Data formatting
The GPS module recieves the data in a formatted string also called as the NMEA sentence, which is a common communication specification used often in naval communications.
Example of NMEA sentences:

[![primjer-NMEA-sentence.jpg](https://i.postimg.cc/KzY128Hk/primjer-NMEA-sentence.jpg)](https://postimg.cc/Lqr9k2R2)

Various data is delimited by a comma and it is the program's goal to extract information from the NMEA sentence string and display it in a valid format.

# Features
Once the power is on, the GPS module automatically tries to search for nearby satellites so it could fetch location data. The LCD display shows the connection status so if it fails the user must restart the connection.
Once the connection is established, the user can select several modes in which different data is displayed. The modes are following:
  - Connection status - SVs is the number of satellites active and FIX is the flag that represents the connection status
    
    [![FIX.png](https://i.postimg.cc/tJCY9Cvn/FIX.png)](https://postimg.cc/0MF8fxs9)
    
  - Location coordinates
  
    [![Koordinate.png](https://i.postimg.cc/TPLjXQ5v/Koordinate.png)](https://postimg.cc/GBRTFFjX)

  - UTC time 
    
    [![UTC-vrijeme.png](https://i.postimg.cc/vms8QZc8/UTC-vrijeme.png)](https://postimg.cc/DSx36FrR)
    
  - Velocity (in knots)
  
    [![Brzina.png](https://i.postimg.cc/bvpP7VBs/Brzina.png)](https://postimg.cc/bZC4bg8h)
    
  - Altitude
    
    [![Visina.png](https://i.postimg.cc/8k9SpzY8/Visina.png)](https://postimg.cc/6TrSztwz)
    
  - Angle azimuth
  
    [![Azimut-kuta.png](https://i.postimg.cc/FHg5VgHm/Azimut-kuta.png)](https://postimg.cc/yDdbVRRr)
