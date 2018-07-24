MODEL 2-3:

This model used a data augmentation on 348 monobloc images. You can see which operation we did by opening diagram.svg
The dataset contained 1879 positive images (with at least one monobloc chair with its bounding box) and 4506 negative images for training.

We performed transfer learning, using a ssd_mobilenet_v2 architecture trained on the Coco dataset, minibatches were size 24, learning rate at 0.004, and we stopped the training at step 50 000. 

You can see Tensorboard's graphics by clicking on the three images, taken at the end of the training.


We did not evaluate this model because it was unstable. We forgot to shuffle images during the first step, which made the loss curve oscillating.
That is why this model is very close to model 2-4 about configuration, but 2-4 performs well better.
