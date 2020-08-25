# MaskRCNN_Video

En este proyecto abordaremos la segmentación semantica usando MaskRCNN en imagenes y video. Los repositorios base de este proyecto son los siguiente. El primero de ellos es la implementación para Tensorflow 1, y el segundo repositorio tiene la actualización para Tensorflow 2.
Se realizaron modificaciones para correr la detección usando la cámara web.

    https://github.com/matterport/Mask_RCNN
    https://github.com/akTwelve/Mask_RCNN

## Preparación del entorno

Prepararemos un entorno con python 3.7.7, Tensorflow 2.1.0 y keras 2.3.1

    $ conda create -n MaskRCNN anaconda python=3.7.7
    $ conda activate MaskRCNN
    $ conda install ipykernel
    $ python -m ipykernel install --user --name MaskRCNN --display-name "MaskRCNN"
    $ pip install tensorflow-gpu
    $ pip install tensorflow==2.1
    $ pip install jupyter
    $ pip install keras
    $ pip install numpy scipy Pillow cython matplotlib scikit-image opencv-python h5py imgaug IPython[all]
    $ conda install -c anaconda cudatoolkit
    
## Instalar MaskRCNN

    $ python setup.py install
    $ pip install git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI
    
## Prueba en Jupyter notebook

    $ cd samples
    $ jupyter notebook
    
## Prueba en consola con imagenes y en video

### Con imágenes

    $ cd samples
    $ python imagemask.py
    
### En video

    $ cd samples
    $ python videomask.py
    
    
# Agradecimientos

    Matterport, Inc
    https://github.com/matterport

    Adam Kelly
    https://github.com/akTwelve
