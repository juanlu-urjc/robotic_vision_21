## Welcome to Robotic Vision subject

This blog is about Robotic Vision subject of the Artificial Vision máster of the [Rey Juan Carlos University](http://www.urjc.es) of Madrid. In this website I will be narrating my progress in this subject.
<P align="right">by Juan Luis Carrillo</P>

Specifically, the following exercises have been carried out:
- [Follow Line exersice of Unibiotics platform](#p1)
- [3D Reconstruction](#p2)

### <a name="p2" />3D Reconstruction

In this practice, the [3D Reconstruction](https://jderobot.github.io/RoboticsAcademy/exercises/ComputerVision/3d_reconstruction) exercise of the Robotics-Academy website will be carried out. Specifically, the 3D scene shown below will be reconstructed.

![Escena en 3D]
(https://drive.google.com/file/d/1JS89lrKmcDtGCwj8HqQhwkpPesa6YaEm/view?usp=sharing)

This scene will be reconstructed from the following images.

![Par estéreo](https://drive.google.com/file/d/17roNKSaw5KJP3lDyU5AyxbACDKZZxeIM/view?usp=sharing)

To achieve the objective, the following steps have been followed:
- Perform a Canny filter
- Calculate the epipolar line
- Obtain the homologous points of the two images
- Calculate 3D point from homologous 2D points

#### Perform a Canny filter

The first step has been to apply a Canny filter to the images of the stereo pair, as shown in the following figure.

![Filtro de Canny](https://drive.google.com/file/d/1dkLj6GjVFlDcn0bygPAH32CztUtb93bg/view?usp=sharing)


### <a name="p1" /> Follow Line exersice of Unibiotics platform 

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
