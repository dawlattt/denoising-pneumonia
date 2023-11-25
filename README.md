# denoising-pneumonia
In this project, we are evaluating the impact of denoising techniques like, Convolutional Denoising Autoencoders [CDA](https://github.com/adam-mah/Medical-Image-Denoising), Block Matching 3D, and Wavelet on several classifiers. We have selected AutoML, Logistic Regression, SVM, ResNet50 and Swin Transformer as the models for binary classification of X-Ray Images into normal and pneumonia. These models are trained on the [Chest X-ray Pneumonia dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), and the achieved results were used as a baseline. For training the Machine Learning models we extracted features from the original dataset after training ResNet18 model, where we flattened the last convolutional layer to end up with 512 features for each image, the implementation is found [here](Feature_Extraction) , all weights is found [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/EoFn_5c7Ib1Gnk5mxSn9OdcBnt0CDnBhEZqwjnNE3oeIig?e=nhiOuB).. 

![diagram](https://github.com/dawlattt/denoising-pneumonia/assets/150269995/dcb62888-6cf1-4629-889d-2cff54cfe786)


**Basline**
  - [logistic_regression_baseline.ipynb](Logistic_Regression/logistic_regression_baseline.ipynb)
  - [svm_baseline.ipynb](SVM/svm_baseline.ipynb)
  - [automl_baseline.ipynb](AutoML/automl_baseline.ipynb)
  - [resnet_baseline.ipynb](ResNet50/resnet_baseline.ipynb)
  - [swin_baseline.ipynb](Swin/swin_baseline.ipynb)




**Our next step involved applying different denoising techniques to remove noise from our dataset. The denoising methods we utilized include:**

- **CDA denoiser**
  - For implementation, see [CDA.ipynb](Denoisers/CDA.ipynb).
  - Denoied dataset is available [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/EleswHYsodxNhBVfQknlTTYBSUVkyrrd8ihPkiCFn3emHA?e=1IZ9M4).

- **Bm3d denoiser**
  - For implementation, see [Bm3d.ipynb](Denoisers/Bm3d.ipynb).
  - Denoied dataset is available [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/Es4l41z5vtFKqJ86bEeuFdYBtU2CRlrGcUMYlgf--V4gyQ?e=ypPiE4).

- **Wavelet denoiser**
  - For implementation, see [wavelet.ipynb](Denoisers/wavelet.ipynb).
  - Denoied dataset is available [here](https://mbzuaiac-my.sharepoint.com/:f:/g/personal/dawlat_akaila_mbzuai_ac_ae/EoD-W5BEoEBHodObX0HsTq4BNF83OriRgVpEUrjcqAzg3Q?e=fl6y1j).



**For results after applying the CDA denoiser, please refer to the following files:**
  - [logistic_regression_cda.ipynb](Logistic_Regression/logistic_regression_cda.ipynb)
  - [svm_cda.ipynb](SVM/svm_cda.ipynb)
  - [automl_cda.ipynb](AutoML/automl_cda.ipynb)
  - [resnet_cda.ipynb](ResNet50/resnet_cda.ipynb)
  - [swin_cda.ipynb](Swin/swin_cda.ipynb)

**For results after applying the BM3D denoiser, please refer to the following files:**
  - [logistic_regression_bm3d.ipynb](Logistic_Regression/logistic_regression_bm3d.ipynb)
  - [svm_bm3d.ipynb](SVM/svm_bm3d.ipynb)
  - [automl_bm3d.ipynb](AutoML/automl_bm3d.ipynb)
  - [resnet_bm3d.ipynb](ResNet50/resnet_bm3d.ipynb)
  - [swin_bm3d.ipynb](Swin/swin_bm3d.ipynb)

**For results after applying the BM3D denoiser, please refer to the following files:**
  - [logistic_regression_wavelet.ipynb](Logistic_Regression/logistic_regression_wavelet.ipynb)
  - [svm_wavelet.ipynb](SVM/svm_wavelet.ipynb)
  - [automl_wavelet.ipynb](AutoML/automl_wavelet.ipynb)
  - [resnet_wavelet.ipynb](ResNet50/resnet_wavelet.ipynb)
  - [swin_wavelet.ipynb](Swin/swin_wavelet.ipynb)
  

