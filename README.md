# Fine-tune-a-Segformer
Fine tuning of a Segformer for an agricultural environment

# Motivation/Problem

As an engineering thesis I developed the design and prototype of a mobile robot for greenhouse fumigation which worked according to the objectives set. The navigation system was low level, since it was only guided by routines and distance measurements. As a future work I proposed to integrate a computer vision system to give more capabilities to the developed robot.

# Planning

I limited myself to a quick development, first collect data, label it, apply some preprocessing techniques and then use a pre-trained model. I have also contemplated analyzing the performance of the model in real time, as well as the hardware needed for it (probably a Jetson).

# Data

I personally collected the data with a mobile device in the middle of the day with good lighting conditions and with mature tomato crops. The original images are high resolution (+2000 px).

# Modeling

A Segformer model pre-trained with ImageNet 1K has been selected to experiment with the data; models such as SAM and UNET are planned to be used.

# Deployment

The intention of this model is to deploy it on a frontier device such as a Raspberry or Jetson, currently the model can be used in the HuggingFace repository.

# Tools used

[Segments.ai](http://Segments.ai) was used for labeling as well as HuggingFace for training and deployment.

# Internet resources or bibliography

The original article is the main reference to understand the model: [2105.15203.pdf (arxiv.org)](https://arxiv.org/pdf/2105.15203.pdf)

I followed this tutorial: [Fine-Tune a Semantic Segmentation Model with a Custom Dataset (huggingface.co)](https://huggingface.co/blog/fine-tune-segformer)
