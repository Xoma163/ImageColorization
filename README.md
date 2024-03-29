Дипломная работа на тему "Автоматизированная система колоризации чёрно-белых изображений"
-


### Requirements
- cuda_11.0.2_451.48_win10
- cudnn-11.2-windows-x64-v8.1.0.77
- python 3.8.3

```
SET PATH=C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.0\bin;%PATH%
SET PATH=C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.0\extras\CUPTI\lib64;%PATH%
SET PATH=C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.0\include;%PATH%
SET PATH=C:\tools\cuda\bin;%PATH%
```



### Dataset
[Download 10 000 images](https://andrewsha.net/static/files/images_10k.zip) (~1 GB)

[Download 100 000 images](https://andrewsha.net/static/files/images_100k.zip) (~10 GB)

[Download 64x64 100 000 images for testing](https://andrewsha.net/static/files/images_64x64_100k.zip) (~170 MB)

ToDo
[Download pre-trained model](https://andrewsha.net/static/files/pre_trained_model.zip) ()

Put dataset images in {{IMAGES_ORIGINAL_PATH}} (see in consts)

### Setup 

```
sudo ln -s "$PWD/config/image_colorization.service" /etc/systemd/system/
```

```
sudo ln -s "$PWD/config/nn.andrewsha.net.conf" /etc/nginx/sites-available/ 
sudo ln -s "$PWD/config/nn.andrewsha.net.conf" /etc/nginx/sites-enabled/
```
