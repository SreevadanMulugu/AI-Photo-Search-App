# AI-Photo-Search-App
This program is a photo search app that uses the Qwen2VL model to pull out important keywords from images. It links the keywords to each image so users can search for them as many times as they want. When a search is done, the matching images show up quickly, making it easy to find pictures based on their content.
 Example 

# Other Approaches

PHI 3 VISION INSTRUCT (INT4 QUANTISATION)
onnx-cpu  2 min 40 sec (webp)(overall cpu usage 60-70%)     
onnx-cpu  2 min 36 sec (png)(overall cpu usage 60-70%)
onnx-cuda 5 sec (near instant )

QWEN 2 VL 2B INSTRUCT 
native cpu approximate 600 sec  (10 min) (cpu usage overall 10%)
native cuda 60 sec 

YOLO11
Fastest near instant on cpu and gpu 
Object identification but cannot understand the image and thus inefficient method 

Cuda -NVIDIA RTX 4050 MOBILE GPU
Cpu -Intel i5 (13th gen ) 13420h 8 cores 12 logical processors 

As this models are not that fast and resource intensive(phi 3 cpu ) or more time consuming  (Qwen 2 model) only fast solutions is QWEN 2 Vl (cuda) and phi vision (cuda) but it requires nvidia gpu which is not that affordable and only seen in gaming laptops which are lot less seen than normal computers (non gpu ) as the amount of ram taken by this models are also more we cannot run this models efficiently on edge pc (as the amount of pictures in any device is considerably high) or the computing power should be increased (cpu cores gpu ) which is not feasible to create a on device solution that works within a reasonable time frame . 

But the cuda only ondevice solution can be made and also colab solution can be created as colab resources and gpu is more powerful than consumer grade cpu gpus

