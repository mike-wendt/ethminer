## Build for Ubuntu 16.04

```
sudo apt-get install cmake -y
git checkout volta
mkdir build
cd build
cmake -DETHASHCL=OFF -DETHASHCUDA=ON -DHUNTER_JOBS_NUMBER=8 ..
cmake -DETHASHCL=OFF -DETHASHCUDA=ON -DHUNTER_JOBS_NUMBER=8 --build .
cd ethminer
make
```

### Make Distro

```
cd build/ethminer
mkdir bin
cp ethminer bin/
tar czf ethminer.tgz bin
```
