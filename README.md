# Rocket Flight Simulator

A python application that uses Euler's method to computationally solve the nonlinear, 2nd order differential equation that represents the vertical flight of a rocket. Uses 1st order approximations for atmospheric density and engine thrust data.

![Simulator](https://image.prntscr.com/image/Ll-SqvFVRhaifLjRa7ZVhg.png "Flight Simulator Program")

This program was originally developed as a project for MTE 204 (Numerical Methods) at the University of Waterloo in Fall 2019.

### Installation/Setup
`pip3 install -r requirements.txt`

### Usage
`python3 -m rocket_flight_simulator`

If you get a Qt error about not being able to find the Qt platform plugin xcb, run `sudo apt-get install libxkbcommon-x11-0`.

If using to estimate performance of a custom rocket, modify the parameters and data in `parameters.json` and `thrust.csv`. The paramters currently in both files are for a custom rocket with a G80T-14A motor. `atmosphere.csv` contains atmospheric data taken from the US Standard Atmosphere and should not be modified.

### Running tests
`python3 -m unittest`
