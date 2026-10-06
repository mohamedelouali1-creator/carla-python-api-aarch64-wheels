# CARLA Python API 0.9.13 for ARM64 (aarch64)

Pre-compiled CARLA Python API wheels for **Jetson Nano / ARM64** architecture.

## Files
- `carla-0.9.13-cp38-cp38-linux_aarch64.whl` - Python 3.8 wheel (recommended)
- `carla-0.9.13-py3.8-linux-aarch64.egg` - Python 3.8 egg (legacy)

## Installation

### Option 1: Wheel (recommended)
```bash
pip3 install carla-0.9.13-cp38-cp38-linux_aarch64.whl
```

### Option 2: Egg
```bash
pip3 install carla-0.9.13-py3.8-linux-aarch64.egg
```

## Verify Installation
```python
import carla
print(carla.__version__)  # 0.9.13
client = carla.Client('localhost', 2000)
print("Connected to CARLA server:", client.get_server_version())
```

## Compatibility
| Component | Version |
|-----------|---------|
| **OS** | Ubuntu 20.04 (Focal Fossa) |
| **Python** | 3.8 |
| **Architecture** | aarch64 (ARM64) |
| **Hardware** | Jetson Nano, Jetson Xavier NX, Jetson AGX Xavier, Raspberry Pi 4 |
| **CARLA Server** | 0.9.13+ |

## Usage with ROS 2 Foxy + CARLA ROS Bridge
See [ROS_BRIDGE_JETSON.md](https://github.com/your-repo/jetson-nano-memo/blob/main/ROS_BRIDGE_JETSON.md) for complete setup.

## Source
Built from [carla-simulator/carla@0.9.13](https://github.com/carla-simulator/carla/tree/0.9.13) with ARM64 toolchain.

## License
MIT License - see [CARLA License](https://github.com/carla-simulator/carla/blob/master/LICENSE)
