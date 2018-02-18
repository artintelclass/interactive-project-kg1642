Idea Proposal

I wanted to create based on the movements of the user. After discussing with Professor Sherwood in the class, I decided to use Kinect to monitor the movements of the user. 

Working Prototype

After deciding to use Kinect I borrowed one from the IM lab and started playing around with it. For my working prototype, I focused on changing the pitch of the sound based on far the user is from the Kinect. As the user goes farther the pitch of the sound increases.I set up the wekinator project to output one continous output. It is better to use continous output as pitch is continous.  Click [THIS LINK](https://www.youtube.com/watch?v=RInJLYd5LOk&feature=youtu.be) see the video of my working prototype. Couple of my friends tried the working prototype. Almost all of them suggested me to use more soothign sound, which was my intention after all. One of the friends also asked me to consider using devices other than Kinect has the reputation for crashing from time and again. However, it was dfficult for me to find another input device for distance measuring. 

Final Project
For the final project, I wanted to utilize the 3 dimensional information provided by the Kinect rather than just measuring distance. I found that z value from the Kinect is related to the distance from the Kinect and x and y are related to left and right position from the Kinect. 
My webkinator project took three inputs from the Kinect and send out two continous outputs. First output was trained to higher the more right you go of the Kinect. Second output was trained to increase as you go farther away from the Kinect. 
Now, to make that the output make sensible sounds, I used MIDI which then connected to Sforzando (a piano player). I modified the MIDI processing file to produce the desired sound. The modified file can be found HERE. I modified the file in such a way that the delay between the notes increased as the value of the first output increased (as we go from left to right) and the pitch of the played note increased as the value of the second output increased ( as we go farther from the Kinect). If you are confused, THIS Video might help you understand.  

Requirements to Run this Project:
1. Download or clone this repository on your local machine.
2. Get and Kinect and set it up. You can find more information on how to set up your Kinect [HERE](https://github.com/ml4a/ml4a-ofx/releases)
3. Start a wekinator project which takes in 3 inputs and 2 outputs and choose the All Continous type. Also change the output value from 0-1 to 0-127.
4. Train the model as described above. 
5. Download Sforzando and City-Piano-SFZ. 
6. Run the ProcessingToMIDI_NoteOn_2ContinuousOutputs.pde which is under ProcessingToMIDI_NoteOn_2ContinuousOutputs file. 
7. Now, move around and marvel at how you can produce music with your body movements. 
