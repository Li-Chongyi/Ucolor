# Ucolor
```
This Repo includes the training and testing codes of our Ucolor. (TensorFlow Version).

We also provided a MindSpore version of our code: https://pan.baidu.com/s/152jgursbXgxTEDLNGZ2SIw (password: a5ls).

If you use our code, please cite our paper and hit the star at the top-right corner. Thanks!
```
# Notice
```
In the originally released code, we may upload the incorrect transmission maps in some folders. In the updated version, we have corrected the provided transmission maps and provided the code that can generate the transmission map.  
```

The codes can be found at 
Google Drive: https://drive.google.com/file/d/1c2bjXMKyszogNxgPxQF9mQ9EkRKAbnB6/view?usp=sharing

or

Baidu Cloud: https://pan.baidu.com/s/14t0H9OFpWCZr1ltVNb62PQ  (Password: nseu)



# Requirement
```
Python 3.5.6, TensorFlow 1.6.0, Cuda 9.0.
```

<!---
### Results
```
For your evaluations, we provide all results of our method and the compared methods.
The results can be found at
```
Google Drive: https://drive.google.com/file/d/1zrynw05ZgkVMAybGo9Nhqg2mmIYIMVOT/view?usp=sharing

or 

Baidu Cloud:  https://pan.baidu.com/s/13DyFwlz3aTJ3LGkVOVuOvQ (Password: hyap)
-->

## Testing
```
1. Download the code
2. Put your testing images in the "real_90_input" folder and put the corresponding transmission maps in the "real_90_gdcp" folder (keep the same sizes and names as the images in the "real_90_input")
3. Python main_test.py
4. Find the result in "real_90_input" folder
Note that our method needs extra transmission maps estimated by General Dark Channel Prior (GDCP) as input (GDCP: Generalization of the dark channel prior for single image restoration) 
For your convenience, we provide all paired testing data (input images and corresponding transmission maps) used in our paper. You can find them in the "testing_data_extra" folder.
```
## Training
```
1. Download the code
2. Python main_train.py
3. Find checkpoint in the ./checkpoint/coarse_112

The training data are in the "input_train" folder (underwater images), "depth_train" folder (transmission maps), and "gt_train" folder (ground truth images).
The validation data are in the "input_test" folder (underwater images), "depth_test" folder (transmission maps), and "gt_test" folder (ground truth images).
```

## Bibtex

```
@Article{Ucolor,
          author ={Li, Chongyi and Anwar, Saeed and Hou, Junhui and Cong, Runmin and Guo, Chunle and Ren, Wenqi},
          title = {Underwater Image Enhancement via Medium Transmission-Guided Multi-Color Space Embedding},
          journal = {IEEE Transactions on Image Processing},
          Volume={30},
          pape={4985-5000},
          year = {2021},
          doi={10.1109/TIP.2021.3076367}
          }
```
##  License
The code is made available for academic research purpose only. This project is open sourced under MIT license.

## Contact
If you have any questions, please contact Chongyi Li at lichongyi25@gmail.com.

