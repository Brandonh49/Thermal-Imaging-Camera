# Thermal Imaging Camera
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
| Brandon H | Chadwick School | Hardware Engineering | Incoming Junior |

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 

# First Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/CaCazFBhYKs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


For my first milestone, I had to set up the hardware and software aspects of the project to get the camera fully up and running. The camera itself requires a 3.3V, GND, SDA, and SCL connection to the Raspberry Pi. These connections can be fulfilled without soldering using the Stemma QT cables, though this specific configuration that I am building uses QT to male headers, meaning it cannot be directly connected to the Raspberry Pi. Instead, I used a breadboard and another set of male/female cables to bridge the Pi and camera through the breadboard.

Once this was done, I then used PuTTY (you can use any SSH client) to configure the I2C settings of the Pi through the GUI. This process includes setting the baudrate to the MX90640's max supported rate, 400000, and ensuring any other relevant I2C functions are enabled. Once this was done, I then created a virtual environment for Python and installed the pithermalcam library from PyPi via pip3. This allows me to create a test and run file for the camera, which I then move to a directory of the actual Pi. At this point, the file just needs to be excecuted via the Pi terminal and the basic functionality of the camera should be working.







For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Adafruit MLX90640 IR Thermal Camera Breakout - 55 Degree | Thermal Camera Board/Sensor | $74.95 | <a href="https://www.adafruit.com/product/4407"> Link </a> |
| STEMMA QT / Qwiic JST SH 4-pin to Premium Male Headers Cable - 150mm | Non-solder connection option for camera board | $0.95 | <a href="https://www.adafruit.com/product/4209"> Link </a> |
| Raspberry Pi 4 4GB Starter Kit - 64GB w/ Housing | Raspberry Pi Computer | $104.99 | <a href="https://a.co/d/bKFdsDf"> Link </a> |
| Electronics Kit | General electronics kit | $15.99 | <a href="https://a.co/d/hcAJmUk"> Link </a> |

# Other Resources
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [General Guide] <a href="https://tomshaffner.github.io/PiThermalCam/">

