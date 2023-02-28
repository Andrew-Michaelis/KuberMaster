This app is a basic prebuilt webpage that congratulates you on using a node Docker-Image
the Dockerfile is used entirely to set up the conditions and environment for node
this helps with maintaining version stability regardless of author


To create and run the webpage, first ensure you are in the directory containing the Dockerfile
Ensure that Docker is running on your machine
Use your terminal to execute the commands;
1: docker build .  ###optionaly use {docker build -t [NAME] .} to name the container you are creating
2: docker image ls   ###discover and copy the [ID] of the image you just created, unnecessary if you [NAME]d it
3: docker container run --rm -p 80:3000 [ID]  ###[ID] is replaced with [NAME] if you used the tag feature.
Navigate to localhost:80 in your web browser and view your accomplishment
Return to terminal and terminate the process with CTR-C to stop the program   ### the --rm earlier removes the container on termination
