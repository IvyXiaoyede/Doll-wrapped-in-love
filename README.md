# Doll-wrapped-in-love
My project shows a 3D build of a doll's head and a 2D love image using particle effects. It is 
a combination of 2D and 3D, so I built it using two script statement blocks to separate the 
3D from the 2D.
To start with the doll, I referenced the zdog statement library to build a 3d doll head, in the 
head block I defined the height and position of the doll head so that it is always centred. 
After that it was time to select the canvas and start drawing the doll's head, first determining 
all the colours I needed to use and then anchoring the zdog scene, after which I could use the 
canvas to draw the picture. Because it is a 3D image, I use the z-axis to give the image an 
undulation when I position it so that it looks like a 3D image when it rotates. When drawing 
the right eye, as the image is the same, I chose to copy the left eye directly using the copy 
statement and then adjusted the position to make a right eye. The mouth was made using the 
circle, taking half of the circle and using it as the doll's mouth. The ears are made using the 
cone, the rotating type has to be thick so the cone is made. Finally, I added an animation to 
make the doll rotate from side to side. This is the part of the doll.
The next part is the heart. The heart was added to reflect the concept of a child wrapped in 
love being happy, so instead of using a single painted line when making the heart, I wanted to 
use a particle effect to show it off. When setting up the particles I set the maximum size, 
duration, diameter of the particles and the speed of diffusion; for the particle pool, I first 
created a particle pool and created a circular queue to keep the particles cycling through to 
create a diffusion effect. Of course, there is still a need to constantly update the particles, so 
I set up if statements to allow active particles to appear and then eliminate particles that 
have reached their maximum effect so that there is no redundancy in appearance and the 
sense of boundaries fades away. The next step is to get the particles to combine and draw 
the heart pattern, using cos and sin statements to draw it. The next step is to use the virtual 
canvas to create the particle image, create it on the canvas, then go on to create the path, fill 
and image, finally render the image, set the update time, clear the canvas to create new 
particles, and of course resize the canvas at the end to add a delayed render that will look a 
little smoother.
The above is my interpretation of the project, the idea is to come from a child wrapped in 
love to create a child who will always be wrapped in happiness and luck.
