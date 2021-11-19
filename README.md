## <div align="center">Запустить inference на своем изображении</div>

<details open>
<summary>Install</summary>

[**Python>=3.6.0**](https://www.python.org/) is required with all
[requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) installed including
[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/):
<!-- $ sudo apt update && apt install -y libgl1-mesa-glx libsm6 libxext6 libxrender-dev -->

```bash
$ pip install -r requirements.txt
```
<details open>
<summary>Inference with detect.py</summary>
`detect.py` запустить inference можно для изображения или для видео. Для этого скачайте веса можеди по ссылке 
the [custom_yolo5x.pt](https://drive.google.com/file/d/1-yrHyNpo9g35AlScUB4yDGvcHqTyPORT/view?usp=sharing) результат сохраняется в основную дирикторию.
Если на вход подать изображение с именем 00001.png
В результате, в текущей папке должен появиться файл 00001_out.png, на котором отрисованы bounding box-ы.

```bash
$ python detect.py --source img.jpg  # image
                            vid.mp4 or .mov # video

```