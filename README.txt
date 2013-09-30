6) face_rec

Description : A ROS wrapper for a face tracking program developed by Alexandros Loulemes. The program uses opencv to
capture images from a camera and detect faces, and annotate them with a circle of different colour for each face detected.
The ROS node records the id of each face, its coordinates and the radius of the circle around it. It then proceeds to
publish a message containing this information for each face detected in every frame it processes. The message published is
a vector of messages each containing the above information

To run :

    roslaunch openni_launch openni.launch
    roslaunch face_rec fr.launch User presses START to start tracking and sending messages and the X button to quit the program
