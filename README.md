# 6D Localization

6D pose estimation algorithm for the RoboCup 3D Soccer Simulation League

Video: https://youtu.be/cwb1YUGHXGA

Distributed by FCPortugal under GNU GPLv3

## Requirements

**GNU Scientific Library (GSL):**

* sudo apt install libgsl-dev

**Third-party libraries (or self-made):**

* Singleton.h - Singleton class
* Vector3f.h - 3D vector class with basic vector operations
* Matrix4D.h - 4D matrix class with basic matrix operations
* Globals.h - defines the agent namespace to access agent and ball properties
* RobovizLogger.h - log utility to draw shapes and annotations in RoboViz (https://github.com/magmaOffenburg/RoboViz)

## Usage

```c++
LocalizerV2 loc;
loc.run();
auto m = loc.headTofieldTransform;

//m contains the head to field transformation matrix
```
