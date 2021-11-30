A machine learning model was built to classify spectrum. CNN model was used for the task of graph classification. The model was written in python and used frameworks including Tensorflow and OpenCV. Both notebook and python versions of the code are provided in the ML_model directory.

The model was trained using dataset ftir_library and raman_library downloaded from https://wincowger.shinyapps.io/OpenSpecy/. The trained model is saved in . If you want to train a new model yourself, please run ML_model.py.

You can make predictions of spectrum type from a given graph of wavenumber and intensity by running predict.py. Please change the path to your file location. The default file used for prediction here is testdata.csv downloaded from https://wincowger.shinyapps.io/OpenSpecy/. Top 10 predictions of most likelihood are given.
