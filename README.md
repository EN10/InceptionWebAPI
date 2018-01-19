# Inception API

### API for Google Tensorflow Inception Model

Based on [Quick and Simple Image Recognition](https://github.com/EN10/SimpleInception)

Install
-

    sudo pip install -U pip
    sudo pip install tensorflow

**Download Classifier Program:**    

    wget https://raw.githubusercontent.com/tensorflow/models/master/tutorials/image/imagenet/classify_image.py

Run Model
-

    python classify_image.py --image_file image.jpg

Make API
-
**Classify images from URL Node API:**   

Example:
* https://inception-eniof.cs50.io/?q=http://saxony-blue.com/data/out/86/5918348-image.jpg   

image url is a parameter of page url   

**Download Webserver App:** 

    wget https://raw.githubusercontent.com/EN10/InceptionAPI/master/web.js

**Install Webserver:**  

    npm install express     

**Run Web App:**    

    node web.js

web.js: downloads image using curl then calls classify_image.py on it