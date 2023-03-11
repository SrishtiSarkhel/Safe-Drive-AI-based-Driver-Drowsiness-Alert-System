# Safe-Drive-AI-based-Driver-Drowsiness-Alert-System
•Project Duration: September 2022 to October 2022 

•Summary: In this python project, We have innovated a detection mechanism using python, openCV and Dlib, where in the camera of the car dashboard will detect your face and analyse it, if the driver is found drowsy then an alarm will be played along with that a LED panel will light up to alert the nearby cars. After studying the shortcomings of the upcoming systems we have implemented a mechanism where in, if the alarm is ignored by the driver thrice the details of the driver will be sent to the nearby highway authority, police and hospitals to alert them for some upcoming accident. 

•Problem Statement: 21% of all fatal accidents are due to drowsy driving. 60% of adult drivers or about 168 million people have driven a vehicle while feeling drowsy in the past year. About 37% or 103 million people have fallen asleep at the wheel, according to the National Sleep Foundation's [NSF] 2005 poll.
NHTSA estimates that in 2017, 91,000 police-reported crashes involved drowsy drivers. These crashes led to an estimated 50,000 people injured and nearly 800 deaths.

•Idea/Solution: We have innovated a detection mechanism using python, openCV and Dlib, where in the camera of the car dashboard will detect your face. There are mostly two steps to detect face landmarks in an image which are given below:
  1) Face detection: Face detection is the first methods which locate a human face and return a value in x,y,w,h which is a rectangle.
  2) Face landmark: After getting the location of a face in an image, then we have to move through points inside of that rectangle. Here we are the Dlib’s 68 Facial landmark detection.

•Here, in this code snippet we have a loop from 0 to 27 (we have started here from 0 instead of 1 because in python an index starts from 0 and not from 1) which only traces the facial boundary and hence we can see the yellow dots on the facial boundary, similarly we can follow this for our focus area which will be the eyes.

•How will we find out if the eye is opened or closed?
So we can use a geometrical concept called as the Euclidian distance, as the Euclidian distance between the  points reduces i.e. they tend to 0, my system will alert the driver with a sound alert that the driver is drowsy. 
The values for the eyes opened and closed i.e 0.25 and 0.21 are pre calculated and we are using it for the same.

•How the system will prevent False alarm?
The system won’t warn or play an alarm if the driver is blinking because I have used a if statement where each time the camera detects sleeping eyes it will increment the value of sleep variable by 1 and unless the loop is not repeated for six times, it won’t produce any alarming system. Hence we can avoid false alarm for activities such as blink or sneeze.
               
 •TechStack/Prerequisites:
 1) Python (version 3.10.7)
 2) OpenCV and Dlib (For Facial Recognition and Facial mapping)
 3) Pygame (To play the alarm sound)
 4) Microsoft SQL (For Database Management the Authority End)
 5) Led lamp panel (To alert nearby vehicles)




                
    










