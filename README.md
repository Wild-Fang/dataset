# Data Set
Our image dataset for machine learning

## How we manage Data

We start by preparing the data that you’ll use to train and evaluate the classifier. We create a training data set from about 80% of the images you have for each label. We create a testing data set from the remaining images. The same image should only appear in one dataset.

The 2 separate datasets:
- `training`: 80% of images
- `tests`: 20% of images

Next, we create 2 separate folder for each datasets. In each folder, we create subfolders using your labels as names. Then we sort the images into the appropriate subfolders for each data set.
![How it should look like](https://docs-assets.developer.apple.com/published/4bd09c3420/b789d462-92c2-4d26-9479-d5288eef2438.png)

The exact label strings aren’t important, as long as they make sense. For example, we might use the label Cheetah for all the images of cheetahs. We don’t have to name the image files in any particular way or add metadata to them. The only requirement is to put them into the folder with the right label.

There should be at least 10 images per label for the training set, but more is always better. Also, the number of images for each label should be balanced. For example, we don’t use 10 images for Cheetah and 1000 images for Elephant.

The images can be in any common format. This includes common formats like JPEG and PNG. The images don’t have to be the same size as each other, nor do they have to be any particular size, although it’s best to use images that are at least `299x299` pixels. **If possible, train with images collected in a way that’s similar to how images will be collected for prediction.**

We should only provide images with variety. For example, images that show animals from many different angles and in different lighting conditions. A classifier trained on nearly identical images for a given label tends to have poorer performance than one trained on a more diverse image set.

> Note
> Images should look "real", they have to look like as if they were taken by an iPhone or another camera. We don't want something that was shot to close or an image that could contain ambiguous objects.


