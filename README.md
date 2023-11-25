# denoising-pneumonia
In this project, we are evaluating the impact of denoising techniques like, Convolutional Denoising Autoencoders [CDA](https://github.com/adam-mah/Medical-Image-Denoising), Block Matching 3D, and Wavelet on several classifiers. We have selected AutoML, Logistic Regression, SVM, ResNet50 and Swin Transformer as the models for binary classification of X-Ray Images into normal and pneumonia. These models are trained on the [Chest X-ray Pneumonia dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), and the achieved results were used as a baseline. For training the Machine Learning models we extracted features from the original dataset after training ResNet18 model, where we flattened the last convolutional layer to end up with 512 features for each image. 

![diagram](https://github.com/dawlattt/denoising-pneumonia/assets/150269995/dcb62888-6cf1-4629-889d-2cff54cfe786)


For the baseline, please refer to the following files:

    -[automl_baseline.ipynb]()
    svm_baseline.ipynb
    logistic_regression_baseline.ipynb
    resnet_baseline.ipynb
    swin_baseline.ipynb


Our next step involved applying different denoising techniques to remove noise from our dataset. The denoising methods we utilized include:

- **CDA denoiser**
  - For results, see [CDA.ipynb](Denoisers/CDA.ipynb).
  - Dataset is available [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/EleswHYsodxNhBVfQknlTTYBSUVkyrrd8ihPkiCFn3emHA?e=1IZ9M4).

- **Bm3d denoiser**
  - For results, see [Bm3d.ipynb](link_to_Bm3d.ipynb).
  - Dataset is available [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/Es4l41z5vtFKqJ86bEeuFdYBtU2CRlrGcUMYlgf--V4gyQ?e=ypPiE4).

- **Wavelet denoiser**
  - For results, see [wavelet.ipynb](link_to_wavelet.ipynb).
  - Dataset is available [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/EoD-W5BEoEBHodObX0HsTq4BNF83OriRgVpEUrjcqAzg3Q?e=fl6y1j).


For results after applying the CDA denoiser, please refer to the following files:

    automl_cda.ipynb
    svm_cda.ipynb
    logistic_regression_cda.ipynb
    resnet_CDA.ipynb
    swin_CDA.ipynb

For results after applying the BM3D denoiser, please refer to the following files:

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
    
All weights can be found [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/EoFn_5c7Ib1Gnk5mxSn9OdcBnt0CDnBhEZqwjnNE3oeIig?e=nhiOuB).

