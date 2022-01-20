## Motivation
Data augmentation is widely used as a means of generating more training data from a small initial sample in order to improve model performance. Current popular methods of data augmentation include zooming in on the original image and capturing the original image at different angles. A recent paper (DatasetGAN) takes a slightly different approach to dataset augmentation by utilizing a generative adversarial network to generate labeled (segmented) images from a small initial set.

When performing dataset augmentation, one potential source of issue is that the generated images (and labels) are only as good as the originals. In other words, if there are errors in the original image labeling, data augmentation runs the risk of propagating these errors into a larger dataset. In a study early in 2021, a group at MIT found that up to 3.4% of images in benchmark vision datasets such as CIFAR-100 and MNIST were mislabelled (https://l7.curtisnorthcutt.com/label-errors). This poses a potential issue since training on mislabeled data that is later augmented will compromise the model's ability to solve the target task.

This work sets out to investigate the effects of perturbing the label on original images. Namely, I will run the DatasetGAN model on the image segmentation datasets from the DatasetGAN paper to establish a baseline. Then, I will repeat the process where one of the segmentation labels from the original set of images is altered slightly to determine how much of an effect this perturbation has, and how the degree of perturbation affects the final performance of the model.

## DatasetGAN
DatasetGAN (https://arxiv.org/pdf/2104.06490.pdf) builds upon the StyleGAN architecture to generate labeled images from a small starter set.

## Data perturbation
TODO

## Experiments
TODO