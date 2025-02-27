## Plan
1. Install software that can be used to identify the keypoints
2. Create a list of commands that will need to be transcribed
3. Convert the sign language keypoint configurations into text
4. Connect the code to a robot to recieve commands

# ASL to Robot Commands

Team Members:
- Bianca Burgess, biburges@buffalo.edu
- Piyush Salian, psalian@buffalo.edu

--- 

## Project Objective
The goal of this project is to capture the keypoints in the hand, arm and upper body while a person is speaking in ASL. This will then get translated into text which will then send commands to a robot. This way a deaf person can interact with the robot and send it commands using computer vision. 


## ASL/Robot Command Examples
- Stop
![My Image](Stop.png)
- Start
![My Image](Start.png)
- Down
![My Image](down.png)
- Up
![My Image](up.png)
- Left
![My Image](left.png)
- Right
![My Image](right.png)
- Open (Gripper)
![My Image](open.png)
- Close (Gripper)
![My Image](close.png)


## Contributions
What is unique about this project is that there are lots of people who have created ASL translator devices. This is the glove that detects your hand position and it is connected to a computer that tells you what the person is signing. With this project, it will allow the person to sign to a screen and the computer vision will pick it up the keypoint for it be sent to the robot for its commands.


## Project Plan

### Potential Computer Vision Packages:
MediaPipe
- Open source package by Google that performs hand tracking, pose estimation. This is to be integrated with Tensorflow. Package detects 21 key landmarks per hands and could possibly isolate the hand from the background.
- Use MediaPipe hand tracking to detect hand landmarks
- Extract 21 hand landmarks and use a classifier to train certain hand gestures
  
### ASL-to-Text Processing
NLP models(LSTM/Transformer)
 - Natural Languauge Processing is used to convert ASL
Only applicable for the creation of sentences in ASL, however this is not within the scope of our project. 


### Robot Communication
- ROS 2(not sure which robot to use)(simulation or real arm?)
Via Gazebo, different simulated worlds and models can be loaded up. With the use of ROS syntax and concepts, we can simulate manifestations of ASL inputs into robot arm movements. 

## Milestones/Schedule Checklist
{What are the tasks that you need to complete?  Who is going to do them?  When will they be completed?}
- [X] Complete this proposal document.  *Due Feb. 28*
- [ ] Successfully setup MediaPipe package with dependencies *Due April 1*
- [ ] Successfully extract 21 landmarks through the MediaPipe handmodule *Due April 1*
- [ ] Create progress report.  *Due April 3*
- [ ] Train the model with a classifier *Due April 10*
- [ ] Load the model and perform real-time gesture recognition *Due April 13*
- [ ] Setup Gazebo successfully *Due April 17*
- [ ] Setup simulated robot arm *Due April 19*
- [ ] Write ROS code that interfaces with ASL inputs *Due April 30*
- [ ] Create final presentation.  *Due May 6*
- [ ] Provide system documentation (README.md).  *Due May 13*


## Measures of Success
We believe partial credit should come from the achievement of major milestones in the form of 
1) Succesfully setting up MediaPipe environment, extracting landmarks and training the model to accurately identify gestures
2) Setting up the gazebo simulation to interface with ASL gestures
3) Simulation responds effectively to ASL gestures
