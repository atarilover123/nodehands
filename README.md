# nodehands

NodeHands adds osc to a handtracking sketch from [Creativeguru97](https://github.com/Creativeguru97) - [original code](https://github.com/Creativeguru97/YouTube_tutorial/tree/master/Play_with_APIs/hand_detection/mediapipe_hands/final)

This modification uses node to create a server that sends osc messages from the P5 sketch - xy positions of each trcked hand point. 

### Steps 

1. make sure node is installed. If not installed download and install [Node](https://nodejs.org/en)
2. in the terminal cd to nodehands directory (unzip the folder first, your directory should look like the image below)  
<img width="727" alt="Screenshot 2023-10-10 at 9 42 13 AM" src="https://github.com/atarilover123/nodehands/assets/36606910/d6c20386-ab8e-428d-8ac3-fb150b0994ae">

3. run the bridge.js file
<img width="727" alt="Screenshot 2023-10-10 at 9 45 00 AM" src="https://github.com/atarilover123/nodehands/assets/36606910/f1c936d4-719b-4391-909a-6c1432b6d421">

4. open the index.html file, select a camera. Once this webpage is running sucessfully the terminal should update say "connection"
    
<img width="643" alt="Screenshot 2023-10-10 at 9 47 49 AM" src="https://github.com/atarilover123/nodehands/assets/36606910/f6e4d7fc-7ece-421e-a8a9-e34e79af3d52">

5. you can now read the osc data in other platforms - osc data is broadcasting on port 3334 (example of how to read port 3334 in TouchDesigner using the oscin chop)
6. <img width="1331" alt="Screenshot 2023-10-10 at 9 52 17 AM" src="https://github.com/atarilover123/nodehands/assets/36606910/e548be95-1edc-42da-84b4-fd160b8271e0">


Note:
The point data comes in at x,y coordinates relative to the p5js canvas - 640 * 480. If desired it can be mapped to a usable range in the sketch.js file or by mapping in other software e.g TD, MaxMSP using math and scale objects.  
