# Vehicle 1: Sensor-Driven Motion Simulation

A simulation of Braitenberg's Vehicle 1, built in Unreal Engine. Lab coursework from
my MSc in Artificial Intelligence at BTU Cottbus-Senftenberg.

Vehicle 1 is the simplest machine in Valentino Braitenberg's book *Vehicles:
Experiments in Synthetic Psychology*. It has one sensor and one motor. The sensor
reads a value from the environment, here a temperature gradient, and the motor turns
at a speed proportional to that reading. Nothing steers it. It only goes faster in
warm areas and slower in cold ones, and it keeps whatever direction it started with.

The point of the exercise is what an observer reads into that. A vehicle that speeds
up near a heat source and crawls away from it looks like it wants something, even
though there is no decision anywhere in the design, just one number driving one
motor.

## What the simulation shows

The environment has zones of different temperature. As the vehicle passes through
them, its speed changes with the local reading. With friction switched on it moves
irregularly at low sensor values, sometimes coming to a stop entirely. Without
friction it keeps going and only varies its speed.

## Running it

You need Unreal Engine 5. Clone the repository, open `vehicle1.uproject`, and press
Play. The behaviour is set up in Blueprints, so there is nothing to compile.

## Notes

This is a lab exercise rather than a finished piece of software. The interesting part
is the gap between how simple the mechanism is and how deliberate the movement looks
from outside.
