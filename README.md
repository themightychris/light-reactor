# light-reactor
An experimental art installation that any number of people can create and explore with together

## Project Goals

- Be big, bright, brilliant, and bring people together
- Allow any number of people to affect the system at a time. Instead of a specialized input device that as limited number of people can use at a time--leaving others to observe and wait--the input will be anything that emits bright light
- Provide an obvious baseline link between cause and effect that leads into exploration, discovery, and sharing of more elaborate cause and effect

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
