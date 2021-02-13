#  Neural Style Transfer
Using 

> Thank for the great sharing. Please find the original link is from 2 repo with link below:
[repo1](https://github.com/misgod/fast-neural-style-keras) & [repo2](https://github.com/zaidalyafeai/Fast-Style-Transfer-Keras-TF.js)

## Pre-requisites

You need keras 2 with tensorflow backend 

## Test Prediction 

`python transform.py -i rose.jpg -s la_muse -b 0.1 -o  out`

This will create the output image and a keras .h5 file 

## Conversion of the models 

`tensorflowjs_converter --input_format keras keras.h5 output/`

## Load the model to the browser

This is done using tensorflow.js check the file fast-style.html. Note that I have and editted version of the source package `tf.min.js`. 
It containts many custom layers like corpping and upsampling that are yet to be implemented in tf.js. 
Make sure to use that file. Here is the demo https://tommy-ngx.github.io/fast_style/

![Alt text](Screen-Shot.png?raw=true "Title")

