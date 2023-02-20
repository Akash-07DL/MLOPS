we will detect Person, Face, Mask and helmet in a video or CCTV video and will build a web application with **Streamlit**.

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

Note: For Helemt and Mask part - We didn't tried for very good accuracy as our aim is to simply build a web application which will be running on local host. 

# Detect Helmet:
We will use the cv::dnn::readnet or cv2.dnn.ReadNet() function for loading the network into memory. It automatically detects configuration and framework based on the file name specified. We will give the input trained weight file and the configuration(.cfg) file. For classes we will use obj.names. 


# Detect Mask:
We will use cv2.dnn_DetectionModel. DetectionModel allows to set params for preprocessing input image. DetectionModel creates net from file with trained weights and config, sets preprocessing input, runs forward pass and return result detections. For DetectionModel SSD, Faster R-CNN, YOLO topologies are supported.
