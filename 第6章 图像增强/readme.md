# Updated to do image augmentation 图像增强
```
train_datagen = ImageDataGenerator(
      rotation_range=40,
      width_shift_range=0.2,
      height_shift_range=0.2,
      shear_range=0.2,
      zoom_range=0.2,
      horizontal_flip=True,
      fill_mode='nearest')
```
These are just a few of the options available (for more, see the Keras documentation. Let's quickly go over what we just wrote:

* rotation_range is a value in degrees (0–180), a range within which to randomly rotate pictures. 
* width_shift and height_shift are ranges (as a fraction of total width or height) within which to randomly translate pictures vertically or horizontally.
* shear_range is for randomly applying shearing transformations.
* zoom_range is for randomly zooming inside pictures.
* horizontal_flip is for randomly flipping half of the images horizontally. This is relevant when there are no assumptions of horizontal assymmetry (e.g. real-world pictures).
* fill_mode is the strategy used for filling in newly created pixels, which can appear after a rotation or a width/height shift.


* rotation_range价值度(0 - 180),一个范围内,随机旋转图片。
* width_shift和height_shift范围(如总宽度或高度)的一小部分在垂直或水平随机翻译图片。
* shear_range是随机应用剪切转换。
* zoom_range内随机缩放图片。
* horizontal_flip是随机翻转图像水平的一半。这是有关当没有假设水平assymmetry(如实际照片)。
* fill_mode策略用于填写新创建的像素,后会出现旋转或宽度/高度的转变。
