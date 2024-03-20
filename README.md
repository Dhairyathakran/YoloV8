# YoloV8
Start to End

# Requirements for yolov8
- There two methods ti install yolov8 
1-Install ultralytics==8.0.0

2-you can install via github repo of yolov8

-clone https://github.com/ultralytics/ultralytics.git


# YOLOv8 for Object-Detection via
-yolo task=detect mode=predict model=yolov8n.pt source=Here put the name of image.

when i run this i face this error FileNotFoundError: [WinError 2] The system cannot find the file specified   

we also set the confidence number using conf=0.8
we also save the output using save_txt=True
we also crop the output using save_crop=True
we also hide the Levels and confidence using hide_levels=True , hide_conf=True

if we apply segmentation run this code -yolo task=segment mode=predict model=yolov8n-seg.pt source=Here put the name of image.

if convert the yolov8 model into Onnx format

-yolo mode=export task=detect model=yolov8n.pt format=onnx
