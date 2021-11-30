A machine learning model was built to classify spectrum. CNN model was used for the task of graph classification. The model was written in python and used frameworks including Tensorflow and OpenCV. Both notebook and python versions of the code are provided in the ML_model directory.

The model was trained using dataset ftir_library and raman_library downloaded from https://wincowger.shinyapps.io/OpenSpecy/. The trained model is saved in ML_model/my_model. If you want to train a new model yourself, please run ML_model.py.

When the model is trained for major spectrum types like HDPE, PET, etc, the model can achieve near 100% accuracy for both training and validation dataset. However, when all 536 spectrum types from ftir_library are included, most of which often have only one or two samples to be trained, the overall accuracy would drop to about 58%.

You can make predictions of spectrum type from a given graph of wavenumber and intensity by running predict.py. Please change the path to your file location. The default file used for prediction here is testdata.csv downloaded from https://wincowger.shinyapps.io/OpenSpecy/. It is not preprocessed though, waiting results from the pre-process branch. Top 10 predictions of most likelihood are given.
