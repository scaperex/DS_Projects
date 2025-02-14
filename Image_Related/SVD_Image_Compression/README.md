# SVD Image Compression

## Creates 'compressed' images of lower resolution from a given image.

To reproduce results:

```shell script
conda env create -f svd_compression_environment.yml
conda activate svd_compression
python best_k_approximation.py
```

The original image we took had a height of 576 pixels and width of 768 pixels.

At K =~40 the resulting picture can be clearly understood, but still a little blurry.

At k = ~160 the resulting picture looks almost identical to the original one.

The ratio between the minimal value we found (160) and the rank of the original RBG Matrix (576)
is 160/576 = 0.27 = ~1/4

The following is the full results of the error rate vs the k for each color.

The errors agree with the optimal value of k for general understanding of the picture (meaning big drop error up to k = ~40). 

![results](/Image_Related/SVD_Image_Compression/cute_dog_approximation_results3.png)
![images](/Image_Related/SVD_Image_Compression/results_images_5,10,40,80,160_.jpg)