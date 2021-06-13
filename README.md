# Problem Statement
The main idea of this project is to build a pen which can sense and store the data written through it conserving the texture of written data which could be further accesed by the device connected with the pen.

## Ideation
Just like a mouse this pen keeps the record of previous state and compare it with its new state to find its new location and path covered by it hence we want to keep track of location of the tip as well as the environment around it (SLAM) in order to compare its new position.
This functionality is well mamnaged by a mouse It consist of an LED and its rays are directed by a small prism on the surface on which mouse is kept these rays are reflected and further pass through a lens which converges it onto CMOS sensor which takes around thousand of images per second and send to DSP (Digital Signam Processing) which processes the image and find it's new location and makes cursor move in similar fashion.

CMOS:-This sensor consists of millions of pixels which when exposed to light turns photons to charge this accumulated charged is turned into voltage and gets amplified simuntaneously within the pixel and every such voltage is assigned with corrosponding colour that fell on that pixel (photon).

![Untitled](https://user-images.githubusercontent.com/82231782/121818501-3cffcf80-cca5-11eb-80a8-be2af08ca8fa.png)

IMPROVEMENTS THAT CAN BE MADE:-

1. Instead of using tredition red LED used in mouse we can use IR led since having a pen with countinuously glowing LED is very distracting and is not favoured .Far better advantage of using IR LED is that it consumes less power that's why most of the remotes used IR LED incresing the battery life.

2. It is not a good idea to keep the pen working (ON) all the time since it is going to drain the bettery quickly and can also add unwanted text that the user didn't intended to write for eg going to next line or changing the page at that instant the pen is still recording the text to avoid this we can introduce pizoelecteric sensors into the pen. Pezo electric sensor generates electrical charge and can be measured as voltage difference when it experiences pressure. Hence when ever the pen touches the surface of paper the inbuilt pizoelectric sensor will sence the pressure abd starts recording the text.
