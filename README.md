# celestronController

This is a simple python/kivy serial control application to change the azimuth and altitude on a Celestron NexStar SE Telescope Mount. 


The NexStar Communication Protocol v1.2 as detailed in: https://s3.amazonaws.com/celestron-site-support-files/support_files/1154108406_nexstarcommprot.pdf
is the basis for the mess in nexstar.py, which is an attempt at not making as much of a spaghetti code mess compared to some other things I've written.

To run, have the telescope remote connected via usb serial port to the controller machine. 

Keep CelestronControlApp.py and nexstar.py in the same directory 

Run:
python CelestronControlApp.py 

and it should display a kivy window with the current time and buttons for  ±AZ/ALT control at speeds of 9,6, and 1.

other parts of the GUI are not yet working.



This will be run on a Raspberry Pi to remotely control the telescope via VNC.
