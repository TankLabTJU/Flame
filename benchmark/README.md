# Real Benchmarks in Flame's Evaluation
The real benchmarks used in Flame's evaluation.
The applications in the benchmarks are collected from ServerlessBench and FunctionBench. By configuring different memory sizes and input parameters for these applications, we expand the size of the benchmark pool to 384 functions. 

The application name consists of the function ID and its functionality, e.g., case9-matmul. These functions run on the OpenFaas platform and the handle.py is the entry function. We built a local storage service to replace the existing S3 API in our code. The dataset directory contains the files that the function needs to download, including pictures, text, and videos.

These functions are run with Python 3.4 (ML applictions in tensorflow:1.4.1), we list the necessary requirements in the following:

```
pip install exifread minio
pip install pillow
pip install six
pip install chameleon
pip install numpy
pip install ops
pip install opencv-python
pip install Scikit-learn==0.20.4
```




