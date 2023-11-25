# denoising-pneumonia
In this project, we are evaluating the impact of denoising techniques on several pneumonia classifiers. We have selected AutoML, Logistic Regression, SVM, ResNet50 and Swin Transformer as the models for our classifiers. These models were previously train on the [Chest X-ray Pneumonia dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), and the achieved results were used as a baseline. For training the Machine Learning models we extracted features from the original dataset after training ResNet18 model on our data, where we flattened the last convolutional layer. 

Our next step involved applying different denoising techniques to remove noise from our dataset. The denoising methods we utilized include:

    CDA denoiser (for results, see CDA.ipynb)
    Bm3d denoiser (for results, see Bm3d.ipynb)
    Wevelet denoiser (for results, see wavelet.ipynb)

After removing noise, we retrained our models, but this time on denoised images.

For the baseline, please refer to the following files:

    automl_baseline.ipynb
    svm_baseline.ipynb
    logistic_regression_baseline.ipynb
    resnet_baseline.ipynb
    swin_baseline.ipynb

For results after applying the [CDA denoiser](https://github.com/adam-mah/Medical-Image-Denoising), please refer to the following files:

    automl_cda.ipynb
    svm_cda.ipynb
    logistic_regression_cda.ipynb
    resnet_CDA.ipynb
    swin_CDA.ipynb

For results after applying the Bm3D denoiser, please refer to the following files:

    automl_bm3d.ipynb
    svm_bm3d.ipynb
    logistic_regression_bm3d.ipynb
    resnet_bm3d.ipynb
    swin_bm3d.ipynb


For results after applying the Wavelet denoiser, please refer to the following files:

    automl_wavelet.ipynb
    svm_wavelet.ipynb
    logistic_regression_wavelet.ipynb
    resnet_wavelet.ipynb
    swin_wavelet.ipynb
