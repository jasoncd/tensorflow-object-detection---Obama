# Tensorflow Object Detection -- Find Obama In Photos

# Data
The data used in the experiment can be downloaded from  

     https://www.kaggle.com/jipingsun/object-detection-obama
     
# Requirements

Environment:
The experiment is done on Linux (Ubuntu 16.04 with GPU Cuda library version 9.0, cudnn version 9.0, Tensorflow 1.5 GPU version)

Installation:

(1) Install Google tensorflow library located at

     https://github.com/tensorflow/models
        
   Navigate to the folder: models/research/object_detection
   
(2) Merge the folder 'object_detection' of this repo

(3) Prepare the data set and copy the generated train.record and test.record to the folder 'object_detection'

(4) Obtain the Google model at 

    http://download.tensorflow.org/models/object_detection/faster_rcnn_inception_v2_coco_2018_01_28.tar.gz

and extract it to the sub-folder 'object_detection/faster_rcnn_inception_v2_coco_2018_01_28

# Training and Testing

In object_detection folder, execute 

  ./run-train and then execute 
  
  ./run-test  (choose either image or webcam option inside the script)
  

(Note: in training/ folder, edit the path "find_tune_checkpoint:" of the file pipeline.config to suit the path of the Google model)

# Results

Detection accuracy is around 95%.



