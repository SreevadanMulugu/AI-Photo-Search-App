# AI-Photo-Search-App
This program is a photo search app that uses the Qwen2VL model to pull out important keywords from images. It links the keywords to each image so users can search for them as many times as they want. When a search is done, the matching images show up quickly, making it easy to find pictures based on their content.
 Example 
 ![image](https://github.com/user-attachments/assets/41d12189-5aed-4bd1-ac6b-cc20bd34f7d1)
 ![image](https://github.com/user-attachments/assets/52674036-326b-47fb-819a-06b164a180fa)
 ![image](https://github.com/user-attachments/assets/c22ba0f4-9175-41d9-9417-6f4131512a94)
 ![image](https://github.com/user-attachments/assets/17a07c3c-c1d9-41d9-b11e-a8c998613b60)






# Other Approaches

### Performance Summary of Other AI Models

- **PHI 3 Vision Instruct (INT4 Quantization)**
  - **ONNX (CPU)**: 
    - WebP: 2 min 40 sec (60-70% CPU usage)
    - PNG: 2 min 36 sec (60-70% CPU usage)
  - **ONNX (CUDA)**: Near-instant, approximately 5 sec

- **Qwen 2 VL 2B Instruct**
  - **Native (CPU)**: ~600 sec (10 min, 10% CPU usage)
  - **Native (CUDA)**: 60 sec

- **YOLO11**
  - Fast, near-instant performance on both CPU and GPU
  - Efficient for object identification but lacks image understanding

### Hardware Specifications
- **CUDA**: NVIDIA RTX 4050 Mobile GPU
- **CPU**: Intel i5 (13th Gen) 13420H, 8 cores, 12 logical processors

### Insights
- **Model Performance**: 
  - Qwen 2 VL (CUDA) and PHI Vision (CUDA) are the fastest solutions but require an NVIDIA GPU, which is often found in gaming laptops.
  - Most consumer-grade computers lack the necessary GPU power, making it difficult to run resource-intensive models efficiently.

- **On-Device Limitations**: 
  - Due to high RAM requirements and the number of images stored, running these models on edge PCs is not feasible without enhanced computing power (additional CPU cores or a GPU).
  
- **Potential Solutions**:
  - A CUDA-only on-device solution is feasible.
  - A Google Colab solution can leverage more powerful resources, providing better performance than typical consumer-grade CPU GPUs.
