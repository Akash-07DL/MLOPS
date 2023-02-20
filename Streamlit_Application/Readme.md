we will detect Person, Face, Mask and helmet in a video or CCTV video.

# Detect Person:
For Person detection we will use pre-trained official YOLOV3 weight. We will use ImageAI. 

## ImageAI: 
**What is ImageAI?**
ImageAI is a python library built to empower developers, reseachers and students to build applications and systems with self-contained Deep Learning and Computer Vision capabilities.

For More: https://imageai.readthedocs.io/en/latest/index.html

Instantiating the object detection model. Setting the model type as YOLOV3 and giving the weights path to the model object. Then we are customising it only for person with the **obj_detect.CustomObjects(person=True)**.


# Detect Face:
We will use DeepFace library for Face Detection.

