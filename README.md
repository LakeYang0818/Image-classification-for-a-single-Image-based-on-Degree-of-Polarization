# Image-classification-for-a-single-Image-based-on-Degree-of-Polarization

This project aims at detecting the material (plastic/chong/metal) based on one image:

![alt text](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/45eca0018d56cfa042cf4d992781d3940f6a3c28/Image%20Source/Source_Image.png)

Step 1. Prepare dataset: [Transfer images to npy file.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Transfer%20images%20to%20npy%20file.ipynb)

- Dividing the image into three parts: plastic, chong, metal. [Image Source](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/tree/dcf7677addf482ff254499fca88f5dc893602ba4/Image%20Source).

- Transfering the source image and three material images into .npy files. [Dataset](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/tree/dcf7677addf482ff254499fca88f5dc893602ba4/Dataset).


Step 2. Polarize the three images: [Polarization.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Polarization.ipynb)

- Polarize the image using the Neural Network: [Polarized Images](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/tree/dcf7677addf482ff254499fca88f5dc893602ba4/Polarized%20Images).

Mueller矩阵是一个4x4矩阵, 描述偏振光与各种光学元件或材料相互作用时的变换, 将输入的偏振状态与与光学系统相互作用后的输出偏振状态联系, 考虑了偏振元件（如延迟器、偏振片和波片）的效应。矩阵元素描述了经过光学系统后入射光的Stokes参数（强度、线偏振度、线偏振角、圆偏振度和圆偏振角）如何改变。

Mueller矩阵的一般形式：
M = | I_xx I_xy I_xc I_xs |
    | I_yx I_yy I_yc I_ys |
    | I_cx I_cy I_cc I_cs |
    | I_sx I_sy I_sc I_ss |
    
I_xx，I_xy等: 是对应于不同偏振分量的矩阵元素。
I_xx: 表示与交互后的x方向光强度。
I_xy、I_xc和I_xs: 表示x方向上线性和圆偏振状态的变化，依此类推。

Step 3. Train-Test-Split to prepare datasets for image classification: [Slicing for train data.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Slicing%20for%20train%20data.ipynb)


Step 4. Image Classification [Image Classification.ipynb](https://github.com/LakeYang0818/Image-Classification-for-Polarized-Image/blob/1eebdfecae882fef05f1cbadbea0bf1a2543ed50/Scripts/Image%20Classification.ipynb)
