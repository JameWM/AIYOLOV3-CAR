# By : Warit Mahitti

```
I brought a project of a foreigner to build on. Which I don't remember what his name is, but I will give credit later. I have modified the old version of the code to be the newest version in 2022. I added a function to detect distance lines and measure the speed of The car and I have trimmed the model to be more efficient, both saving CPU, GPU and removing unnecessary functions and IOT.
```

# Multi-type_vehicles_flow_statistics
According to YOLOv3 and SORT algorithms, counting multi-type vehicles. Implemented by Pytorch.  
Detecting and tracking the vehicles in \["bicycle","bus","car","motorbike","truck"].

## Reference
- yolov3-darknet  https://github.com/pjreddie/darknet
- yolov3-pytorch  https://github.com/eriklindernoren/PyTorch-YOLOv3
- sort https://github.com/abewley/sort

## Dependencies
- ubuntu/windows
- cuda>=10.0
- python>=3.6
- `pip3 install -r requirements.txt`

## Usage
1. Download the pre-trained yolov3 weight file [here](https://pjreddie.com/media/files/yolov3.weights) and put it into `weights` directory;  
2. Run `python3 app.py` ;
3. Select video and double click the image to select area, and then start;
4. After detecting and tracking, the result video and file are saved under `results` directory, the line of `results.txt` with format \[videoName,id,objectName] for each vehicle.