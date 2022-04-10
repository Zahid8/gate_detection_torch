# Underwater Object (Gate) Detection using Pytorch

## Overview

This repository created to train a model (Pre-trained Faster R-CNN ResNet-50 FPN Model)and detect an underwater object using pytorch API with the help of [Detecto](https://github.com/alankbi/detecto/).

See works with other frameworks: [tensorflow](https://github.com/enesdemirag/gate-detection/tree/tensorflow), [openCV](https://github.com/enesdemirag/gate-detection/tree/openCV). 

## Getting Ready

#### 1. Install [Detecto](https://detecto.readthedocs.io/en/latest/usage/quickstart.html#installation)

```
pip3 install detecto
```

#### 2. Get your images for dataset.

#### 3. Use [labelimg](https://github.com/tzutalin/labelImg) to label images.

```
pip3 install labelImg
```

#### 4. Run below codes to convert xml files.

```
from detecto.utils import xml_to_csv
xml_to_csv('path_to_xml_folder/', 'labels.csv')
```

## Training

#### Local

- Train on your PC, run [this](training.py) script.

#### Server

- Train on a powerful machine, run [colab notebook](training.ipynb) on Google Colab.

## Testing

- Test using openCV, run [this](testing.py) script.
