## xView Data Utilities for Small Object Detection

This repository is a copy of the original xView dataset for satellite imagery, and the work is part of the Air Force Labs Summer Faculty Research project (SFFP-2020). There are two main branches one is the data_utilities, and the other is the model. The data_utilities has been updated to train images for YOLO4. The model directory (**under construction**) has the files to train the XView dataset for small objects using pre-trained YOLO4 weights. 

The script 'process_wv.py' is runnable and processes a folder containing xView imagery along with a groundtruth geojson file to create a TFRecord containing shuffled, chipped, and augmented xView patches in JPEG format.  We provide several augmentation functions in 'aug_util.py' for rotating and shifting images and bounding boxes, as well as noise injecting techniques like salt-and-pepper and gaussian blurring.  Additionally in 'wv_util.py' we provide several functions for loading, processing, and chipping xView data.

The Jupyter Notebook provided in this repository interactively illustrates an example xView processing pipeline using the provided utility functions.
