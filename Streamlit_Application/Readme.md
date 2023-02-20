we will detect Person, Face, Mask and helmet in a video or CCTV video.

# Detect Person:
For Person detection we will use pre-trained official YOLOV3 weight. We will use ImageAI. 
### ImageAI: 
**What is ImageAI?**
ImageAI is a python library built to empower developers, reseachers and students to build applications and systems with self-contained Deep Learning and Computer Vision capabilities.
Instantiating the object detection model. Setting the model type as YOLOV3 and giving the weights path to the model object. Then we are customising it only for person with the **obj_detect.CustomObjects(person=True)**.
For More: https://imageai.readthedocs.io/en/latest/index.html


# Detect Face:
We will use DeepFace library for Face Detection.
**What is DeepFace?**
DeepFace is the most lightweight face recognition and facial attribute analysis library for Python. The open-sourced DeepFace library includes all leading-edge AI models for face recognition and automatically handles all procedures for facial recognition in the background.
Deepface has a custom face detection function in its interface. We can also use the library with its wide face detector portfolio only with the purpose of performing face extraction. 

Here we used the detector backend as "retinaface", it is slow but up to the mark accuracy.
Read more at: https://viso.ai/computer-vision/deepface/


# Detect Helmet:



# Detect Mask:

