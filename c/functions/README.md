### !!! Please refer to the [README.md](../../README.md) file in the parent directory for configuring the basic environment and obtaining the latest SDK

### [Building programs on Windows](./README-windows.md)

# Building programs on linux


### !! If our camera driver and OpenCV library are not installed, please refer to this tutorial [linux_install_opencv_Driver](../../doc/linux_install_opencv_Driver.md)

### 1. Create a `build` directory in the `functions` directory and navigate into the `build` directory

```Shell
 mkdir build
 cd build
```

### 2. Generate Makefile files using CMake

```Shell
cmake ..
```

### 3. Execute the Makefile to generate the executable file

```Shell
make
```
All executable files will be generated in the 'build' directory

### 4.  Execute the example
```Shell
./open_basic.exe -c ../IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg
```
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