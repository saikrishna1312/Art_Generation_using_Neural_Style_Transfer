# Art Generation using Neural Style Transfer (NST) with TensorFlow

This project implements Neural Style Transfer (NST) using TensorFlow and VGG19, allowing you to blend the artistic style of one image with the content of another. 

Introduction
Neural Style Transfer is a technique used to apply the style of one image (such as a famous painting) to the content of another image. This project utilizes the VGG19 model to extract the style and content features, optimizing a generated image to minimize the differences in content and style between the content and style images.

Key Goals:
- Extract high-level content from the content image.
- Extract style from the style image using the Gram matrix.
- Combine these features to generate a new, stylized image.

How It Works
- Content Image: The image you want to preserve the structure of (e.g., a photograph).
- Style Image: The image whose artistic style you want to apply (e.g., a famous painting).
- Generated Image: The result that combines the content of the content image and the style of the style image.
  
The core idea of NST is to optimize the generated image by minimizing two types of losses:
- Content Loss: Ensures that the generated image retains the structure of the content image.
- Style Loss: Ensures that the generated image captures the style (textures, patterns) of the style image.
- The VGG19 model, pre-trained on ImageNet, is used to extract content and style representations from these images.

Features
- Neural Style Transfer using VGG19 architecture.
- Pretrained ImageNet weights for style and content feature extraction.
- Adjustable hyperparameters for controlling content vs style balance.
- Image size can be customized to fit different needs.
- Output generation and saving of intermediate results at defined intervals.
