## Welcome to Robotic Vision subject

This blog is about Robotic Vision subject of the Artificial Vision máster of the [Rey Juan Carlos University](http://www.urjc.es) of Madrid. In this website I will be narrating my progress in this subject.

### Follow Line exersice of Unibiotics platform 

The goal of [Follow Line](https://unibotics.org/academy/exercise/follow_line/) exercise is to perform a PID reactive control capable of following the line painted on the racing circuit.

To perform the exercise it is necesary to previously do:
1. Pull the latest RADI image from Docker using the following command: docker pull jderobot/robotics-academy
2. Start the Docker container of the image and keep it running in the background (replace "container_name" with a name of your preference): docker run -it --name=container_name -p 8080:8080 -p 7681:7681 -p 2303:2303 -p 1905:1905 -p 8765:8765 jderobot/robotics-academy (In case you've already had the container just run docker run "container_name")
3. Click the connection button and wait until it turns green.
4. Now you can use the exercise!


Then, I program the code using Python language. I use a PD controller and adjust the params to get a loop in 40 seconds.


# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/juanlu-urjc/robotic_vision_21/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
