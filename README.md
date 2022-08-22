# Giraffe Detections

Over the last couple pf years, various giraffe species have become endangered. 2 subspecies have been listed as critically endangered and several others labeled endangered. Using Giraffe Detections, technology can detect and record the presence of giraffes in different areas of the wild to help scientists and experts better protect these animals. 

Making the project
1. Log into nvidia after plugging in the jetson nano kit. Make a new directory:
   mkdir my-detection

2. Then make a new file called Giraffe-Detection.py using the folowing command: 
   nano Giraffe-Detection.py

3. In the file, copy the following code in these images:
   ![2022-08-21 (5)](https://user-images.githubusercontent.com/111521162/185803596-31222f53-349d-4a38-85d9-0674316f38c5.png)
   ![2022-08-21 (6)](https://user-images.githubusercontent.com/111521162/185803608-933fae51-9a21-48d3-ad8c-47d795e9c2fe.png)

Running the project
1. Run the following command (change the "/dev/video0" according to your camera device), which will run the code in the file and save it in an mp4 file:
   python3 Giraffe-Detection.py /dev/video0 output_giraffe.mp4

2. Ctr C to stop running the code.

3. Every time the giraffe was detected, the sentence "A giraffe has been detected" should be written.
![2022-08-21 (4)](https://user-images.githubusercontent.com/111521162/185803739-a06b6dbc-9c47-4641-bf0f-703518c0cf3b.png)

4. At the end, check for the sentence "camera detected giraffes () times." This will not represent the number of giraffes detected, but how many times the camera had        detected a giraffe, which will simply suggest that a giraffe has appeared in a certain area.
![2022-08-21 (3)](https://user-images.githubusercontent.com/111521162/185803743-456f6806-60c8-40b5-af28-9a7744cfdb23.png)

5. To view the mp4 file on your host computer, exit the nvidia and run the command:
   scp nvidia@(type in your own):~/my-detection/output_giraffe.mp4 downloads
   
6. Check your downloads folder to view the video.
