# ISL
Irish Sign Language - Hand shape dataset (ISL-HS)

The ISL-HS dataset contains real hand imagea composed of 26 hand gestures, including 23 static (English alphabet except ’J’, ’X’ and ’Z’) and 3 dynamic gestures (’J’, ’X’ and ’Z’). The typology is one-handed finger spelling. 

To build this dataset, short videos were filmed. In total 6 people (3 males and 3 females) performed the finger spelling ISL alphabets. Each shape was recorded 3 times. 

Each static gesture (hand shape) was performed by moving the arm in an arc from the vertical to the horizontal position. This was performed to simulate rotated gestures that can occur in real word conversations. For the dynamic gestures there was no rotation, only the motion of the gesture. The videos were converted into frames. Frames were converted to grayscale and the background was removed from the frame using a pixel-value threshold. This produced frames that contain only the arm and the hand.

The number of frames for each video depends on its length. Videos were recorded at 30 frames per second (fps) and a resolution of 640 × 480 pixels. The device used to record the videos was an Apple iPhone 7. The videos were saved with .mov extention. The video format is RGB24. In total, dataset contains 468 videos. From these videos a total of 58,114 frames, consisting of 52,688 frames for the static shapes and 5,426 for the dynamic gestures.

Directory's structure:
Videos are stored in different folders, one for each person, consisting of Person1, Person2, Person3, Person4, Person5 and Person6. Inside each folder there are 78 files being 3 for each alphabet letter. File name is given by letter followed by 1, 2 or 3 between brackets. This number represents the shot. For example: "a (1).mov" means shape "a" first shot. 

Frames are stored into different zip files, one for each person. The file name structure is "Person" + person's number + shape + shot number + frame number, separated by hyphen (-). For example, "Person1-A-1-1.jpg" refers to Person 1, shape A, first shot, first frame. 
