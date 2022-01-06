This project is a tool to help transform the instance segmentation mask generated by unityperception into a polygon in coco format.

You can use unityperception to create synthetic masks of 3D models, instance segmentation or semantic segmentation. Currently unity does not release coco data format, this project is to facilitate users to convert the data format to coco format when training deep learning using synthetic data. If you like please give me stars, thanks.

Also, I wanna give an example for testing:

Here is the googledriver link that includes ground-turth and instance segmentation image, use the tool to transfer the mask into coco format for DCNNs training. https://drive.google.com/drive/folders/1nVt6AQDwCGoqNF7jf3ai2KSbLN2TC9xa?usp=sharing


Below are some problems you may meet.
There may be a problem when you use the datasets for training instance segmentation CNNs: You may get error in evaluation for instance segementation, like "File "pycocotools/_mask.pyx", in pycocotools._mask.frPyObjects cvat | Exception: input type is not supported.", 
because there are some seg [] in evaluation json file, please remove them, using replace [], .

If OSError: Could not find library geos_c or load any of its variants ['libgeos_c.so.1', 'libgeos_c.so'] Installed shapely using pip, and had the same problem. 
So I went ahead and installed it like so: sudo apt-get install libgeos-dev in Ubuntu os.
