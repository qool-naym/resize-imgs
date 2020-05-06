# Batch Resizing Images

Short Python script using OpenCV for resizing multiple images. Intentionally to be used for preparing lots of squared images for dataset compiling. You can specify and run the script directly in Terminal. Processes JPG and PNG files and outputs JPGs.

### What you need to do:

Clone repo, pip install requirements, cd to repo directory and put all your source images there.<br/>
Inside the repo dir run ```$ python img_batch_res.py -d [resized_dimensions] -fn [new_file_name]``` .<br/>
If you're running on Python 3 run ```$ python3 img_batch_res.py -d [resized_dimensions] -fn [new_file_name]``` .<br/>

The script will output count of images, processing time, resized dimensions and the destination path.<br/>
Images will be named like so: ```new_file_name00001```, ```new_file_name00002``` etc., adding 5 digits to the<br/>
specified file name.<br/>
Dimensions default to ```512``` and filename defaults to ```image-```.<br/>
If you need more than five digits you can change ```zfill(5)``` in ```img_count = str(counter).zfill(5)```in line 34<br/>
to any positive integer.
