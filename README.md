# Image-classification-for-one-single-Image-based-on-Degree-of-Polarization

This project aims at detecting the material (plastic/chong/metal) based on one image:

![alt text](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/45eca0018d56cfa042cf4d992781d3940f6a3c28/Image%20Source/Source_Image.png)

Step 1. Prepare dataset: [Transfer images to npy file.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Transfer%20images%20to%20npy%20file.ipynb)

- Dividing the image into three parts: plastic, chong, metal. [Image Source](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/tree/dcf7677addf482ff254499fca88f5dc893602ba4/Image%20Source).

- Transfering the source image and three material images into .npy files. [Dataset](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/tree/dcf7677addf482ff254499fca88f5dc893602ba4/Dataset).


Step 2. Polarize the three images: [Polarization.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Polarization.ipynb)

- Polarize the image using the Neural Network: [Polarized Images](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/tree/dcf7677addf482ff254499fca88f5dc893602ba4/Polarized%20Images).


Step 3. Train-Test-Split to prepare datasets for image classification: [Slicing for train data.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Slicing%20for%20train%20data.ipynb)


Step 4. Image Classification [Image Classification.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Image%20Classification.ipynb)
