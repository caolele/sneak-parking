# Sneak-Parking
Bothered by the fact that it is generally difficult to find a parking slot around 
where I live, I hence had the attempt of detecting available parking space using some 
deep learning models. Decided to give it a real quick shot after seeing 
[this post](https://medium.com/@ageitgey/snagging-parking-spaces-with-mask-r-cnn-and-python-955f2231c400).

## Prerequisites
```
conda create -n MaskRCNN python=3.6
pip install -r requirement.txt
pip install git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI
git clone https://github.com/matterport/Mask_RCNN.git
cd Mask_RCNN
python3 setup.py install
```
Download the pre-trained models from [here](https://github.com/matterport/Mask_RCNN/releases);
and copy it into folder ``models``.

Sadly, running jupyter notebook from within a conda environment does not imply your notebook also 
runs in the same environment. Thankfully, there’s an easy fix for that, namely nb_conda, 
and you’ll get it using:
```
conda install nb_conda
```

### Validate basic Mask-RCNN
```
jupyter notebook
```
Open ``scripts/mask-rcnn-healthcheck.ipynb``
