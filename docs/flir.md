# Flir

There is configuration file located in src/v4l2_camera/v4l2_camera.yaml.
It should be copied to another directory called config/

```bash
mkdir config
cp src/v4l2_camera/v4l2_camera.yaml config/
```

Then you need to change the "camera_info_url" field to match your system.

The driver can be run with

```bash
ros2 run v4l2_camera v4l2_camera_node --ros-args --params-file src/v4l2_camera/v4l2_camera.yaml
```
