# Project Proposal
## Idea
Use keypoints in your hand, arm and upper body to while a person is speaking in ASL. This will then get translated into text which will then send commands to a robot. This way a deaf person can interact with the robot and send it commands using computer vision.

## Plan
1. Install software that can be used to identify the keypoints
2. Create a list of commands that will need to be transcribed
3. Convert the sign language keypoint configurations into text
4. Connect the code to a robot to recieve commands

## Software

### Computer Vision for ASL Recognition
1. MediaPipe
2. OpenPose
- Good for full body tracking

### Machine Learning for ASL Recognition
- TensorFlow
- PyTorch

### ASL-to-Text Processing
-NLP models(LSTM/Transformer)
 - Natural Languauge Processing

### Robot Communication
- ROS 2

## ASL/Robot Command Examples
- Stop
- Start
- Down
- Up
- Left
- Right
- Open (Gripper)
- Close (Gripper)
- Reset
