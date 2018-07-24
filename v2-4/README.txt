MODEL 2-4:

This model used a data augmentation on 348 monobloc images. You can see which operation we did by opening diagram.svg
The dataset contained 1879 positive images (with at least one monobloc chair with its bounding box) and 4506 negative images for training.

We performed transfer learning, using a ssd_mobilenet_v2 architecture trained on the Coco dataset, minibatches were size 24, learning rate at 0.004, and we stopped the training at step 50 000. 

You can see Tensorboard's graphics by clicking on the three images, taken at the end of the training.

You can also see the result of an evaluation by clicking on index.png
What do we evaluate? We check that the model predicts well if a monobloc chair is present on the image. 
We do not care about if it finds every monobloc chair on the picture, or if it draw the bounding box correctly.
We just want it finds at least one chair if there is one.