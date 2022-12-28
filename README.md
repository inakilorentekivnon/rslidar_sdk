# TESTING ROBOSENSE (Ubuntu 20.04, Ros2 Humble)

 
Dentro del workspace en `src`:

1. Obtener `rs_driver` mediante `submodule`:

```sh
git clone -b ros2 https://github.com/inakilorentekivnon/rslidar_sdk 
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
git clone -b release https://github.com/RoboSense-LiDAR/rslidar_msg
```
4. Compilar:

```sh
colcon build --symlink-install
```
