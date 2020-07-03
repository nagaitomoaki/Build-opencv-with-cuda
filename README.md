# Building OpenCV library with CUDA
This is for those who have trouble in building OpenCV library with CUDA.

## Version
* OpenCV 3.1
* CUDA 10.1

## CMake
    cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local
    -D WITH_CUDA=ON -D ENABLE_FAST_MATH=1 -D CUDA_FAST_MATH=1 -D
    WITH_CUBLAS=1 -D BUILD_PROTOBUF=OFF -D BUILD_opencv_dnn=OFF -D
    INSTALL_PYTHON_EXAMPLES=ON -D ENABLE_PRECOMPILED_HEADERS=OFF -D
    BUILD_PROTOBUF=OFF -D BUILD_opencv_dnn=OFF -D BUILD_PERF_TESTS=OFF
    -D WITH_TBB=OFF　-D CUDA_TOOLKIT_ROOT_DIR=/usr/local/cuda-10.1 -D
    CUDA_ARCH_BIN='6.1 6.2' -D CUDA_ARCH_PTX="" -DENABLE_CXX11=ON -D
    BUILD_opencv_cudacodec=OFF -D WITH_QT=ON -D WITH_GTK=ON ..
