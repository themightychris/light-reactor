# light-reactor

An experimental art installation that any number of people can create and explore with together. A window into a mirror world where light users provide on their own is reflected as living particles.

## Project Goals

- Be big, bright, brilliant, and bring people together
- Allow any number of people to affect the system at a time. Instead of a specialized input device that as limited number of people can use at a time--leaving others to observe and wait--the input will be anything that emits bright light
- Provide an obvious baseline link between cause and effect that leads into exploration, discovery, and sharing of more elaborate cause and effect

## Vision

### Level 1: Reflection

A projection surface in a dark area is accompanied by various light-emmitting objects. Holding one of these items (or any of your own like a phone, flashlight, flame, etc) before the projection surface produces a particle-based "reflection" on the wall mirroring the general size/shape/color of the input. Moving an item around reveals to the user that the projection acts as a mirror, and any number of people or objects can be reflected at the same time. The particle appearance and behavior may vary by color, lending different "personalities" to different colors.

### Level 2: Painting

Individual tracked inputs, or the entire surface, can be switched into a "painting" mode where the particles remain for an extended but finite period of time before dissipating. Participants can collectively paint a scene that evolves as others join in and old traces expire and fade out. An administrator might flip the whole installation between painting and reflection mode, or individual sources might activate their own trail through a simple gesture.

### Level 3: Living objects

Certain color and shape combinations are recognized and transformed into animated and/or interactive higher-order objects on the surface that persist for an amount of time. For example, a blue circle might create a bubble that floats around and can be popped by a certain other color. A yellow circle might create a smiling sun that rises to the top. A stick figure might come to life and dance idly. A white circle filled in with red and blue might turn into a beach ball that can be bounced around the screen by any source not in painting mode. Users might discover these objects accidentally, learn about them through word of mouth, or pick up hints from "ghost tracers" the system displays occasionally.

### Level 4: Scripted stories and games

Certain objects/gestures or combinations thereof might activate scripted stories or games. Two stick figures might dance together, or a screen-wide game of breakout or pong might activate for a period of time.


## Roadmap

### Proof-of-concept

1. Detect blobs of light against a dark background from a single camera
2. Paint simple circle markers on output stream at detected position with X-axis reversed
3. Color markers with average color of detected blob
4. Use approximate shape of detected blob instead of simple circle markers (optional)
5. Emit simple particles instead of painting shape
6. Enable toggling painting mode globally through administrative control (or setting particle life to arbitrary #s of seconds)

### Enhancements

#### Noise Elimination

1. Capture a neutral image and use diff of current frame with neutral image for blob detection
2. Use blob detection from 2 or 3 cameras to calculate 3d position of light sources and eliminate all blobs outside stage zone


## Technologies and Tools

- [openFrameworks](http://openframeworks.cc/) seems to provide the best combination of performance, flexibility, and usable code
