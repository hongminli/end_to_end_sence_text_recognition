# end to end sence text recognition
This repo implements the end-to-end sence text recognition. The sence text recognition is divided into two steps：
1. Text localization     
(You can see the complete code for text localization in this [repo](https://github.com/THUliumeng/EAST).)  
2. Text recognition    
(You can see the complete code for text recognition in this [repo](https://github.com/THUliumeng/crnn.pytorch).)  
## File structure  
1. east：the necessary files for text localization, include the pretrained model for text localization.  
2. crnn：the necessary files for text recognition, include the pretrained model for text recognition.  
3. end_to_end.py： implement the end_to_end scene text recognition.  
## Installation  
To run this repo, you need the below environment:  
1. tensorflow
2. pytorch
3. opencv
4. numpy  
...and some other packages you need to install according to the error information.    
## Run this repo
1. Put your test image in the directory ./test_img and name it as img_demo.jpg.    
![img_demo](/test_img/img_demo.jpg)
2. Make a folder output, and make empty output.txt and word_area_img folder under the output directory.  
3. Run python end_to_end.py.    
Then you will find the localization result image in ./output/img_demo.jpg. And the result of coordinates in ./output/img_demo.txt.   
![img_demo](/output/img_demo.jpg)  
And the extracted text area images in ./output/word_area_img/word_area_img*.png.  
![word_area_img1](/output/word_area_img/word_area_img1.png) ![word_area_img2](/output/word_area_img/word_area_img2.png) ![word_area_img3](/output/word_area_img/word_area_img3.png) ![word_area_img4](/output/word_area_img/word_area_img4.png)   
And the recognition result in ./output/output.txt and the terminal you use.  
lt  
vehicles  
beware  
of  
  
Congratulations!!!
