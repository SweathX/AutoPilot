# Autonomous Cars Circuit Simulation

A dynamic visualization of multiple self-driving cars navigating a complex circuit using sensor-based navigation and proportional control.

[![Regarder la vidéo](https://img.youtube.com/vi/VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=7DevXKsIlr0)

## Features

- 🚗 **Multiple Autonomous Vehicles** - 3 cars with different colors/speeds navigating independently
- 🛣️ **Complex Circuit Design** - Customizable closed-loop track with multiple curves
- 🧭 **Proportional Control System** - PID-inspired steering adjustment mechanism
- 📡 **Virtual Distance Sensors** - Visualized sensor beams for path detection
- 🌈 **Dynamic Visualization** - Smooth animations with gradient background

## How It Works

### Sensor System

Each car uses a front-mounted virtual sensor that:

1. Projects 40px ahead of vehicle
2. Measures distance to nearest track edge
3. Calculates deviation from ideal path

### Control Mechanism

The navigation system implements:

- **P (Proportional) Control**:

steering_angle = -Kp \* sensor_error

- `Kp`: Proportional gain constant (0.005)
- `sensor_error`: Signed distance from path (negative=left, positive=right)

### Path Following

1. Vector projection calculates nearest point on track
2. Cross product determines deviation direction
3. Continuous steering adjustments maintain optimal path

## Technical Details

**Core Technologies**:

- HTML5 Canvas for rendering
- Vanilla JavaScript for simulation
- RequestAnimationFrame for smooth animation

## Teams

 - Clément Dreiski
 - Mathéo Beaunez


**Key Algorithms**:

- Linear vector projection
- Cross product for direction detection
- Parametric path following
