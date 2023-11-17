# denoising-pneumonia
In this project, we are evaluating the impact of denoising techniques on several pneumonia classifiers. We have selected ResNet50 and Swin Transformer as the architectures for our classifiers. These architectures were previously employed to train models on the Chest X-ray Pneumonia dataset (https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), and the achieved results were used as a baseline.

Our next step involved applying different denoising techniques to remove noise from our dataset. The denoising methods we utilized include:

    CDA denoiser (for results, see CDA.ipynb)
    BM3 
    Kalil's denoiser

After removing noise, we retrained ResNet50 and Swin Transformer, but this time on denoised images.

For the baseline, please refer to the following files:

    resnet_original.ipynb
    swin_original.ipynb

For results after applying the CDA denoiser, please refer to the following files:

    resnet_denoised.ipynb
    swin_denoised.ipynb
