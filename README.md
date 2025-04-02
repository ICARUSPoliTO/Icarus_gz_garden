To set gazebo up:
- from terminal:
  sudo apt update <br />
  sudo apt install libgz-sim7-dev rapidjson-dev <br />
  sudo apt install libopencv-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev gstreamer1.0-plugins-bad gstreamer1.0-libav gstreamer1.0-gl
- clone the repo
- set environment variables:
  GZ_VERSION=garden <br />
  GZ_SIM_RESOURCE_PATH=\<folder path\>/worlds:<folder path>/models <br />
  GZ_SIM_SYSTEM_PLUGIN_PATH=\<folder path\>
- from terminal, in gazebo's folder:
  cmake . -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_POLICY_VERSION_MINIMUM=3.5  <br />
  make

To start a simulation:<br />
    gz sim -v4 -r \<world name\>.sdf <br />

For further details check the documentation in RA_ControlSystem
