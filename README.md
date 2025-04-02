To set gazebo up:
- from terminal:
  sudo apt update
  sudo apt install libgz-sim7-dev rapidjson-dev
  sudo apt install libopencv-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev gstreamer1.0-plugins-bad gstreamer1.0-libav gstreamer1.0-gl
- clone the repo
- set environment variables:
  GZ_VERSION=garden
  GZ_SIM_RESOURCE_PATH=<folder path>/worlds:<folder path>/models
  GZ_SIM_SYSTEM_PLUGIN_PATH=<folder path>
- from terminal, in gazebo's folder:
  cmake . -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_POLICY_VERSION_MINIMUM=3.5
  make

To start a simulation:
    gz sim -v4 -r <world name>.sdf

For further details check the documentation in RA_ControlSystem
