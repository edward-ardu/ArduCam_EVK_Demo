### !!! Please refer to the [README.md](../../README.md) file in the parent directory for configuring the basic environment and obtaining the latest SDK



### [Building programs on linux](./README.md)
# Building programs on Windows

### !! If our camera driver and OpenCV library are not installed, please refer to this tutorial [windows_install_opencv_Driver](../../doc/windows_install_opencv_Driver.md)

### 1. Navigate to the 'functions' directory for testing in Windows PowerShell.

```Shell
cd .....\ArduCam_EVK_Demo-master\c++_\functions
```

### 2. Specify the ArduCam library directory and OpenCV library directory using vcpkg.

- Note: 
   - C project uses "-Darducam_evk_sdk_DIR=..."
   - C++ project uses "-Darducam_evk_cpp_sdk_DIR=..."

```Shell
cmake -Bbuild -DCMAKE_BUILD_TYPE=Release "-Darducam_evk_sdk_DIR=D:/source/repos/evk_demo/evk_sdk/lib/cmake/arducam_evk_sdk" "-DOpenCV_DIR=D:\Opencv\4.6\opencv\build"
```
### 3. Generate the executable file `*.exe` using CMake
```Shell
cmake --build build --config Release
```
All generated executables will be in the `build\Release` directory

### 4. Execute '*.exe' in Windows PowerShell
Navigate to the `build\Release` directory

```Shell
 cd .\build\Release\
```

Execute the desired executable file with the format: " `./executable_filename.exe`    `parameters` "

```Shell
.\open_basic.exe -c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg
```

### 5. Alternatively, you can open `build\Project.sln` and run the project in `Visual Studio`



# Parameters required for the executable file

### capture
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
-n 5 # "Number of times"
```

### capture_async
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
-y 11.36 # "Delay"
```

### capture_async
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
-n 10 # "Number of times"
```

### list_mode
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
-m 1 # "mode"
-o 0 # "only list (1 or 0) Default is closed (0)"
```

### open_advanced
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
-d 1 # "DMA (1 or 0) Default is open (1)"
```

### open_basic
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
```

### open_device
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
-v 2 # "device"
```

### set_transfer_option
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
-t 10 # "count"
-s 1024 # "size"
-n 20 # "Number of times"
```
### show_fps
```Shell
-c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg # "Configuration file name"
```
