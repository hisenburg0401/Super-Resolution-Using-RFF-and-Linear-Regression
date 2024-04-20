# Super-Resolution-Using-RFF-and-Linear-Regression
Begin by exploring the instructor's notebook(https://github.com/nipunbatra/ml-teaching/blob/master/notebooks/siren.ipynb) that introduces the application of Random Fourier Features (RFF) for image reconstruction. Demonstrate the following applications using the cropped image from the notebook:

Superresolution: Perform superresolution on the image shown in notebook to enhance its resolution by factor 2. Show a qualitative comparison of original and reconstructed image.
The above only helps us with a qualitative comparison. Let us now do a quantitative comparison. First, skim read this article: https://github.com/sgrvinod/a-PyTorch-Tutorial-to-Super-Resolution
1) Start with a 400x400 image (ground truth high resolution).
2) Resize it to a 200x200 image (input image)
3) Use RFF + Linear regression to increase the resolution to 400x400 (predicted high resolution image)

Compute the following metrics:
RMSE on predicted v/s ground truth high resolution image
Peak SNR

Completing Image with Random Missing Data: Apply RFF to complete the image with 10%, 20%, and so on up to 90% of its data missing randomly. Randomly remove portions of the data, train the model on the remaining data, and predict on the entire image. Display the reconstructed images for each missing data percentage and show the metrics calculated above. What do you conclude?.
