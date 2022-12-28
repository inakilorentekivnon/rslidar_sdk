# TESTING ROBOSENSE (Ubuntu 20.04, Ros2 Humble)

 
Dentro del workspace en `src`:

1. Obtener `rs_driver` mediante `submodule`:

```sh
git clone https://github.com/inakilorentekivnon/rslidar_sdk/tree/ros2
cd rslidar_sdk
git submodule init
git submodule update
```


2. Instalar dependencias:

```sh
sudo apt-get update
sudo apt-get install -y libyaml-cpp-dev
```


```sh
sudo apt-get install -y  libpcap-dev
```

3. Obtener `rslidar_msg` (rama dev_opt):

```sh
git clone https://github.com/RoboSense-LiDAR/rslidar_msg/tree/dev_opt
```
4. Compilar:

```sh
colcon build --symlink-install
```
