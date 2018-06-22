# VGG-Image-Annotator-Json-Merger
simple notebook to merge vgg json files

[read the blog post](http://azadehkhojandi.blogspot.com/2018/06/first-step-in-object-detection.html) 

In computer vision and image processing, object detection is a process of detecting instances of semantic objects of a certain class/group such as humans, cats, dogs, buildings, cars and so on in digital images and videos.

To build an Object detection model, you need a dataset of tagged/labelled images. Your model learns by examples, It looks into each image in your dataset and then looks up the areas (bounding boxes or polygons) you tagged.

For example here, I wanted to build a model to detect my dog [@cookietheStaffy](ttps://www.instagram.com/cookiethestaffy/) in the photos. 
I tagged the areas that my dog is in the photo and labelled it.

![alt text](https://2.bp.blogspot.com/-fLpjALYIenI/WyxCb1Ac8HI/AAAAAAAACYA/jWsJQx1_3XgF91tx3a9n_H8iAmYw6aaZwCLcBGAs/s640/taggedcookie.PNG "tagged image sample")


There are many tools that you can use for tagging images like

[https://github.com/Microsoft/VoTT](https://github.com/Microsoft/VoTT)
[http://www.robots.ox.ac.uk/~vgg](http://www.robots.ox.ac.uk/~vgg)
[https://www.labelbox.com/](https://www.labelbox.com/)


I used VGG to tag my images. You can export the JSON result of your tagged images easily.

![alt text](https://3.bp.blogspot.com/-JxdmAEI7iFE/WyxSY8Bu70I/AAAAAAAACYM/iwyqoSWfK2w7FKWY5T0FZnJVy01_qaGdACLcBGAs/s640/taggingtool2.PNG "export json")

In the real-world scenarios, you might have thousands of images that you want to label. Obviously,  it's not a one-person job.
My advice is before tagging you need to make sure all the images have a unique name. Then, split your images into small batches and tag them and then export the JSON object for each batch.

With this script you can merge all of the tagged images and the exported JSON results into one file.

https://github.com/Azadehkhojandi/VGG-Image-Annotator-Json-Merger/blob/master/jsonmerge.ipynb
