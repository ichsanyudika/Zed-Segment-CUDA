## Requirements

- ZED SDK

- ZED Camera (ZED / ZED Mini / ZED 2)

- OpenCV ≥ 4.x

- CUDA Toolkit (GPU)

- CMake

### How to Use

- Connect ZED Camera

- Build & Run
  
        mkdir build && cd build
        cmake ..
        make
        ./zed-segment_CUDA
  
- Adjust HSV Use trackbars to fine-tune Hue, Saturation, and Value for segmentation.

- Press q or ESC to quit.

### Results

![](output/output.png)


