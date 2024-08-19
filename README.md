# Person-Tracking-DJI-Tello
This code is an update of an algorithm for detecting and tracking people using posenet models
The code works using posenet models, which detect key points on a person's body. To maintain movement stability, the algorithm uses PID control.
PID control can be fine-tuned to obtain better results.

# Requirements/Setup  
### TelloPy:
Allows you to easily send commands and receive video from the drone. Can be easily installed running:
```bash
pip install tellopy
```
### OpenCV-Python:
```bash
pip install opencv-contrib-python
````
### Simple PID:
Basic PID controler
```bash
pip install simple-pid
````
### Tensorflow:
The base code developed by [@Matthewjsiv](https://github.com/Matthewjsiv) used version 1.15, which was updated to version 2.

### Posenet-Python
For pose detection, I use this python port (made by [@rwightman](https://github.com/rwightman)) of the Tensorflow.js Posenet models created by Google.

### Usage

To start the script, run `track_person.py` with admin privileges. The automatic control is on from the start, but you can toggle it as well as control the drone manually using the keyboard controls below:

- **T** - toggle automatic control
- **Space** - take off (it won't take off automatically)
- **L** - land
- **Q** - rotate counter clockwise
- **E** - rotate clockwise
- **D** - move right
- **A** - move left
- **W** - move forward
- **S** - move backward
- **R** - reset commands (hover/attempt to stay still)
