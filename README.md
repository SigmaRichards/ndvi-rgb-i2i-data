# Paired NDVI/RGB Sentinel Imagery -- Data for Image-to-image translation

This repository contains the processed data used in our paper on image-to-image translation. The dataset contains modified Copernicus Sentinel data (acquired 2023) processed by [Sentinel Hub](https://www.sentinel-hub.com/). Use of Copernicus Sentinel data is subject to the legal notice available [here](https://sentinel.esa.int/documents/247904/690755/Sentinel_Data_Legal_Notice).

The data contains paired and processed satellite NDVI and RGB images. The locations are randomly selected regions throughout Australia. The NDVI images have been rescaled to give positive values a larger range than negative values.

As the pairs of images are prepared as single `.png` files, they are provided side-by-side. The left half of the image contains the True-Colour RGB, while the right half contains the (scaled) NDVI values. All channels in the NDVI image are equal. Each image is contained in `data.zip` in one of the subdirectories (`train`, `val`, `test`) according to subset.

The image counts for subsets are as follows:
 - `train`: 7988 image pairs
 - `val`: 1274 image pairs
 - `test`: 1478 image pairs
