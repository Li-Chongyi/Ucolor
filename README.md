# Ucolor
```
This Repo includes the training and testing codes of our Ucolor. (TensorFlow Version).
The codes can be found at 
```
Google Drive: https://drive.google.com/file/d/1aqI0mRpv5wIh-oq8dP-ZFBhD7zJ7NilZ/view?usp=sharing

or

Baidu Cloud: 

# Requirement
```
Python 3.5.6, TensorFlow 1.6.0, Cuda 9.0.
```

### Results
```
For your evaluations, we provide all results of our method and the compared methods.
```
Google Drive: https://drive.google.com/file/d/1zrynw05ZgkVMAybGo9Nhqg2mmIYIMVOT/view?usp=sharing

or 

Baidu Cloud:  


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
1. Clone the repo
2. Download the VGG-pretrained model from Dropbox: https://drive.google.com/open?id=1asWe_rCduu6f09uiAz_aEP4KAiuoVSRS or Baidu Cloud: https://pan.baidu.com/s/1seDVBooFkmaJ6qF5kuAIsQ (Password: c0nj) (It's preparing for perception loss.)
2. Set the network parameters, including learning rate, batch, weights of losses, etc., according to the paper
3. Generate the preprocessing training data by using the "generate_training_data.m" in folder named generate_test_data
4. Put the training data to corresponding folders (raw images to "input_train",  WB images to "input_wb_train", GC images to "input_gc_train", HE images to "input_ce_train", Ground Truth images to "gt_train"); We randomly select the training data from our released dataset. The performance of different training data is almost same
5. In this code, you can add validation data by preprocessing your validation data (with GT) by the "generate_validation_data.m" in folder named generate_test_data, then put them to the corresponding folders (raw images to "input_test",  WB images to "input_wb_test", GC images to "input_gc_test", HE images to "input_ce_test", Ground Truth images to "gt_test")
6. For your convenience, we provide a set of training and testing data. You can find them by unziping "a set of training and testing data". However, the training data and testing data are diffrent from those used in our paper.
5. Python main_.py
6. Find checkpoint in the ./checkpoint/coarse_112
```

# Contact Us
If you have any questions, please contact us (lichongyi25@gmail.com or lichongyi@tju.edu.cn).



## Bibtex

```
@inproceedings{Ucolor,
 author = {},
 title = {},
 booktitle = {},
 pages    = {},
 month = {},
 year = {}
}
```

## Contact
If you have any questions, please contact Chongyi Li at lichongyi25@gmail.com.

