### !!! Please refer to the [README.md](README.md) file in the parent directory for configuring the basic environment and obtaining the latest SDK

### [Building programs on Windows](./README-windows.md)

# Building programs on linux


### !! If our camera driver and OpenCV library are not installed, please refer to this tutorial [linux_install_opencv_Driver](doc/linux_install_opencv_Driver.md)

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
./open_basic -c <path/config-file-name>
```
# Parameters required for the executable file

### capture
```Shell
-c  # "Configuration file name"
-n  # "Number of times"

./capture -c <path/config-file-name> -n 5
```

### capture_async
```Shell
-c  # "Configuration file name"
-y  # "Delay"

./capture_async -c <path/config-file-name> -y 11.36
```

### capture_async
```Shell
-c  # "Configuration file name"
-n  # "Number of times"

./capture_async -c <path/config-file-name> -n 10
```

### list_mode
```Shell
-c  # "Configuration file name"
-m  # "mode"
-o  # "only list (1 or 0) Default is closed (0)"

./list_mode -c <path/config-file-name> -m 1 -o 0
```

### open_advanced
```Shell
-c  # "Configuration file name"
-d  # "DMA (1 or 0) Default is open (1)"

./open_advanced -c <path/config-file-name> -d 1
```

### open_basic
```Shell
-c  # "Configuration file name"

./open_basic -c <path/config-file-name>
```

### open_device
```Shell
-c  # "Configuration file name"
-v  # "device"

./open_device -c <path/config-file-name> -v 2
```

### set_transfer_option
```Shell
-c  # "Configuration file name"
-t  # "count"
-s  # "size"
-n  # "Number of times"

./set_transfer_option -c <path/config-file-name> -t 10 -s 1024 -n 20
```
### show_fps
```Shell
-c  # "Configuration file name"

./show_fps <path/config-file-name>
```