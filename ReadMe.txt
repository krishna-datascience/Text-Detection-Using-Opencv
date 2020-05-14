Firstly You Have To Install Some Reavent Packages/Modules:

pip install opencv-python
pip install opencv-contrib-python
pip install argparse == 1.1
pip install imutils==0.5.3
- - - - - - - -- - - -- - - - - - -- - - - - - -- - -- -- - - -- -- 
pip install tensorflow ==2.0
pip install keras == 2.3.0

Project structure
To start, be sure to grab the source code + images to today’s post by visiting the “Downloads” section. 
From there, simply use the tree  terminal command to view the project structure:

OpenCV Text Detection (EAST text detector)
$ tree --dirsfirst
.
├── images
│   ├── car_wash.png
│   ├── lebron_james.jpg
│   └── sign.jpg
├── frozen_east_text_detection.pb
├── text_detection.py
└── text_detection_video.py
1 directory, 6 files
Notice that I’ve provided three sample pictures in the images/  directory. You may wish to add your own images collected with your smartphone or ones you find online.

We’ll be reviewing two .py  files today:

text_detection.py : Detects text in static images.
text_detection_video.py : Detects text via your webcam or input video files.
Both scripts make use of the serialized EAST model (frozen_east_text_detection.pb ) 

-----------------------------------------------------------------------------

How To Run:
Run via CMD command Prompt
python text_detection_video.py -- east frozen_east_text_detection.pb

#python text_detection_video.py - - east frozen_east_text_detection.pb