# Mask2polygon_tool
This project is a tool to help transform the instance segmentation mask generated by unityperception into a polygon in coco format.

You can use unityperception to create synthetic masks of 3D models, instance segmentation or semantic segmentation. 
Currently unity does not release coco data format, this project is to facilitate users to convert the data format to coco format when training deep learning using synthetic data. If you like please give me stars, thanks.

Also, I wanna give an example for testing:

Here is the googledriver that link includes ground-turth and instance segmentation image, use the tool to transfer the mask into coco format for DCNNs training. 
https://drive.google.com/drive/folders/1nVt6AQDwCGoqNF7jf3ai2KSbLN2TC9xa?usp=sharing
