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
-c  # "Configuration file name"
-n  # "Number of times"

./capture -c IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg -n 5
```

### capture_async
```Shell
-c  # "Configuration file name"
-y  # "Delay"

./capture_async -c IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg -y 11.36
```

### capture_async
```Shell
-c  # "Configuration file name"
-n  # "Number of times"

./capture_async -c IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg -n 10
```

### list_mode
```Shell
-c  # "Configuration file name"
-m  # "mode"
-o  # "only list (1 or 0) Default is closed (0)"

./list_mode -c IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg -m 1 -o 0
```

### open_advanced
```Shell
-c  # "Configuration file name"
-d  # "DMA (1 or 0) Default is open (1)"

./open_advanced -c IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg -d 1
```

### open_basic
```Shell
-c  # "Configuration file name"

./open_basic -c IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg
```

### open_device
```Shell
-c  # "Configuration file name"
-v  # "device"

./open_device -c IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg -v 2
```

### set_transfer_option
```Shell
-c  # "Configuration file name"
-t  # "count"
-s  # "size"
-n  # "Number of times"

./set_transfer_option -c ..\..\IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg -t 10 -s 1024 -n 20
```
### show_fps
```Shell
-c  # "Configuration file name"

./show_fps IMX519_MIPI_2Lane_RAW10_8b_3840x2160_18fps.cfg
```