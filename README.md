# Giraffe Detections

Over the last couple years, various giraffe species have become endangered. 2 subspecies have been listed as critically endangered and several others labeled endangered. Using Giraffe Detections, technology can detect and record the presence of giraffes in different areas of the wild to help scientists and experts better protect these animals. 

Making the project
1. Log into nvidia after plugging in the jetson nano kit. Make a new directory:
   mkdir my-detection

2. Then make a new file called Giraffe-Detection.py using the folowing command: 
   nano Giraffe-Detection.py

3. In the file, copy the following code in these images:
   ![Code1](https://user-images.githubusercontent.com/111521162/185799849-4e8b81cd-455c-4d26-b08d-5d940c91c852.png)
   ![Code2](https://user-images.githubusercontent.com/111521162/185799869-53e61b2f-d8a8-479b-9360-5a862761d696.png)

Running the project
1. Run the following command (change the "/dev/video0" according to your camera device), which will run the code in the file and save it in an mp4 file:
   python3 Giraffe-Detection.py /dev/video0 output_giraffe.mp4

2. Check for the sentence "A giraffe has been detected." in the code to see if the camera detected a giraffe, like below:
   ![Giraffe Detected](https://user-images.githubusercontent.com/111521162/185800333b33dd9bc-8257-4a54-b420-77da8c841693.png)

3. To view the mp4 file on your host computer, exit the nvidia and run the command:
   scp nvidia@<type in your own>:~/my-detection/output_giraffe.mp4 downloads
   
4. Check your downloads folder to view the video.

