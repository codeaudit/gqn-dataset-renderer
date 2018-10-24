# :construction: Work in Progress :construction:
# GQN Dataset Renderer

This is a Python library for building a dataset for GQN and CGQN based on [CUDA raytracer](https://github.com/musyoku/python-rtx).

## Requirements

- Python 3
- OpenCV
    - `pip3 install opencv-python`
- Pillow
    - `pip3 install Pillow`
- tqdm
    - `pip3 install tqdm`
- pybind11
    - `pip3 install pybind11 --user`
- Ubuntu
    - tested on Ubuntu 16.04 / 17.10
- CUDA
    - tested on CUDA 9.1
- NVIDIA GPU
    - tested on GTX 1070 / 1080
- C++14 (gcc-6)

Also, you need Chainer, PyTorch or Keras to download MNIST images.

## Installation

```
make -j4
```

# Shepard-Matzler

![shepard_matzler](https://user-images.githubusercontent.com/15250418/47383748-53496d80-d740-11e8-8db8-e7a25bd1ad5c.gif)

```
python3 shepard_matzler.py -cubes 5 -colors 12 -k 15
```

# Rooms

![anim](https://user-images.githubusercontent.com/15250418/47347087-7e54a280-d6e9-11e8-93db-47dd2b4efaea.gif)

```
python3 rooms_ring_camera.py -objects 3 -colors 12 -k 5
```

# MNIST Dice

![rooms](https://user-images.githubusercontent.com/15250418/47368004-ce4c5d00-d71b-11e8-9834-bf87b128892b.gif)

```
python3 mnist_dice_ring_camera.py -objects 3 -colors 12 -k 5
```

# Using multiple GPUs

```
python3 rooms_ring_camera.py -objects 3 -colors 12 -k 5 -gpu 0 --total-observations 100000 --num-observations-per-file 2000
python3 rooms_ring_camera.py -objects 3 -colors 12 -k 5 -gpu 1 --total-observations 100000 --num-observations-per-file 2000 --initial-file-number 51
```

# Textures

- http://bg-patterns.com/?p=1607
- http://bg-patterns.com/?p=221
- http://www.everydayicons.jp/patterns/japanese_circle.html
- http://thepatternlibrary.com/#fancy-pants
- http://thepatternlibrary.com/#the-illusionist
- http://thepatternlibrary.com/#maze