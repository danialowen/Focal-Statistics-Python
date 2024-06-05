# Focal Statistics (Moving Window) in Python

This is an example of how to do focal statistics in Python for raster data / numpy array. In this moving window approach, I want to calculate the `SUM` of all *unique* values specified by a custom window (weights matrix). To do this with raster data, use `rasterio` to open the file and use the `read()` function to convert to read the raster as a numpy array.   

In this example, I have created an example of a raster dataset:

![image](https://github.com/danialowen/Focal-Statistics-Python/assets/43341904/d8a52622-b514-4920-afd0-c1f43299bf72)

For this raster, I want to calculate the `SUM` of all unique values that share a horizontal or vertical border with that cell (not including diagonal cells):

![image](https://github.com/danialowen/Focal-Statistics-Python/assets/43341904/7321404b-868b-4cf8-b25a-641843ae8d94)

The result looks like this:

![image](https://github.com/danialowen/Focal-Statistics-Python/assets/43341904/1a79308b-d0c2-4799-bc7f-6fe18ebc1935) 

![image](https://github.com/danialowen/Focal-Statistics-Python/assets/43341904/2431bf4f-d3d5-4e13-92ad-dd10fad92654)

