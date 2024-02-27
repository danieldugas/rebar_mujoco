## Install

https://github.com/google-deepmind/mujoco/releases/tag/3.0.0

Mujoco just released a bugfix, which means we need to build from source
https://github.com/google-deepmind/mujoco/commit/478ce0c8d8954085303278e074c1d4d0da68e2d1

```
cd ~/Code
rm -rf mujoco
git clone git@github.com:google-deepmind/mujoco.git 
cd mujoco
git checkout 478ce0c
mkdir build
cd build
cmake ..
cmake --build .
mkdir bin/mujoco_plugin -p
cp lib/* bin/mujoco_plugin/
```

## Run

```
~/Code/mujoco-3.0.0/bin/simulate ~/Code/rebar_mujoco/scene.xml
```
