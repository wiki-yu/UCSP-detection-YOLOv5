

## Getting Started

###  1. Setup Environment
#### 1.1 Create Virtual Environment

Create Virtual (Windows) Environment:

```shell script
python -m venv env
.\env\Scripts\activate
```
Notes: recommend VS code as the IDE to run the code, pay attention to the script above is for the CMD terminal

Create Virtual (Linux/Mac) Environment:

```shell script
python -m venv env
source env/bin/activate
```

#### 1.2 Install packages
```shell script
pip install -r requirements.txt
```

###  2. Training
```bash
# Train YOLOv5s on UCSP data for 10 epochs
$ python train.py --img 640 --batch 16 --epochs 10 --data ucsp.yaml --weights yolov5s.pt
```     

### 3. Inference

`detect.py` runs inference on a variety of sources, and the result saving results to `runs/detect`. In the meanwhile, the detection can also be seen after the script running. 

```bash
$ python detect.py --source 0  # webcam
                            file.jpg  # image 
                            file.mp4  # video
                            path/  # directory
                            path/*.jpg  # glob
                            'https://youtu.be/NUsoVlDFqZg'  # YouTube
                            'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
```



