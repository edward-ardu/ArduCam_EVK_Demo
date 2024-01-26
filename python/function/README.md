# Introduction

This is a demo for reading and displaying images with sync/async mode.

## Installation dependence

<!-- git clone https://github.com/ArduCAM/ArduCAM_USB_Camera_Shield_Cpp_Demo.git -->
<!-- cd ArduCAM_USB_Camera_Shield_Cpp_Demo -->

```shell
cd python
pip install -r requirements.txt
```

## Functions

### List Devices

```shell
# run
python -m list_devices
```

### Open

Open Basic

```shell
# show help
python -m open_basic --help
# run
python -m open_basic -c <path/config-file-name>
```

Open Specific Device

```shell
# show help
python -m open_device --help
# run
python -m open_device -c <path/config-file-name> -d <device_index>
```

Open Advanced

```shell
# show help
python -m open_advanced --help
# run
python -m open_advanced -c <path/config-file-name> --dma
```

Set Transfer Option

```shell
# show help
python -m set_transfer_option --help
# run
python -m set_transfer_option -c <path/config-file-name> -t <transfer_count> -s <transfer_size> -n <number_of_frames>
```

### Log

Log Basic

```shell
# run
python -m log_basic
```

Set the environment variable `ARDUCAM_LOG_LEVEL` to change the log level before running.
The `ARDUCAM_LOG_LEVEL` value can be `off`, `error`, `warn`, `info`, `debug`, `trace`.

```shell
# run with environment variable
ARDUCAM_LOG_LEVEL=off python -m log_basic
```

```shell
# run with environment variable
ARDUCAM_LOG_LEVEL=trace python -m log_basic
```

Log Callback

```shell
# run
python -m log_callback
```

Log File

```shell
# run
python -m log_file
```

### Capture

Capture Sync

```shell
# show help
python -m capture --help
# run
python -m capture -c <path/config-file-name> -n <number_of_frames>
```

Capture Async

```shell
# show help
python -m capture_async --help
# run
python -m capture_async -c <path/config-file-name> -d <delay_in_seconds>
```

### Utils

Show fps

```shell
# show help
python -m show_fps --help
# run
python -m show_fps -c <path/config-file-name>
```

List All Modes in Binary Config

> Make sure you have a camera connected

```shell
# show help
python -m list_mode --help
# run, and list all modes in binary config
python -m list_mode -c <path/config-file-name> -l
# run, and switch to a specific mode
python -m list_mode -c <path/config-file-name> -i <mode_id>
```

Controls

> Liat all controls

```shell
# show help
python -m controls --help
# run
python -m controls -c <path/config-file-name>
```