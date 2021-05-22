## Welcome to Robotic Vision subject

This blog is about Robotic Vision subject of the Artificial Vision máster of the [Rey Juan Carlos University](http://www.urjc.es) of Madrid. In this website I will be narrating my progress in this subject.
<P align="right">by Juan Luis Carrillo</P>

### 3D Reconstruction

In this practice, the [3D Reconstruction](https://jderobot.github.io/RoboticsAcademy/exercises/ComputerVision/3d_reconstruction) exercise of the Robotics-Academy website will be carried out. Specifically, the 3D scene shown below will be reconstructed.

![Escena en 3D](https://github.com/juanlu-urjc/robotic_vision_21/blob/gh-pages/docs/Escena.png)

This scene will be reconstructed from the following images.

![Par estéreo](https://github.com/juanlu-urjc/robotic_vision_21/blob/gh-pages/docs/par_estereo.png)



### Follow Line exersice of Unibiotics platform 

The goal of [Follow Line](https://unibotics.org/academy/exercise/follow_line/) exercise is to perform a PID reactive control capable of following the line painted on the racing circuit.

To perform the exercise it is necesary to previously do:
1. Pull the latest RADI image from Docker using the following command: docker pull jderobot/robotics-academy
2. Start the Docker container of the image and keep it running in the background (replace "container_name" with a name of your preference): `docker run -it --name=container_name -p 8080:8080 -p 7681:7681 -p 2303:2303 -p 1905:1905 -p 8765:8765 jderobot/robotics-academy` (In case you've already had the container just run docker run "container_name")
3. Click the connection button and wait until it turns green.
4. Now you can use the exercise!


Then, I program the code using Python language. I use a **PD controller**. After many trials to adjust the controller parameters, a lap is completed in just over 30 seconds. For this solution, it is very important that the **Brain parameter is 30**. Otherwise, the car would be very unstable.

This video shows the result.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=tP3CVYRr85c
" target="_blank"><img src="http://img.youtube.com/vi/tP3CVYRr85c/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="480" height="240" border="10" /></a>
