# tensorflow-yolov4

## Installation
install the project dependencies.

```
# for GPU
pip install -r requirements-gpu.txt
# for CPU
pip install -r requirements.txt
```

## Demo

```bash
# Convert darknet weights to tensorflow
## yolov4
python save_model.py --weights ./weights/yolov4-car_final-416.weights --output ./checkpoints/yolov4-car_final-416 --input_size 416 --model yolov4 

# Run demo tensorflow
# single image
python detect.py --weights ./checkpoints/yolov4-card_final-410-416 --size 416 --model yolov4 --image ./data/val/test1.jpg
# video
python detectvideo.py --weights ./checkpoints/yolov4-card_final-410-416 --size 416 --model yolov4 --video ./data/val/test1.mp4 --output_format MP4V --output result.mp4
```
