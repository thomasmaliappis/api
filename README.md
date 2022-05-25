# Audio Processing and Indexing Project

Before doing anything, you should download IRMAS dataset from this link https://www.upf.edu/web/mtg/irmas and put it in a directory called dataset.

Then, if you run the [process_dataset.ipynb](process_dataset.ipynb) jupyter notebook you will create 4 new files called X_train_data.npy, y_train_data.npy, X_test_data.npy and y_test_data.npy under the dataset directory.
This process takes more than half an hour to complete.

After you have created these files you can run the [instrument_classifier.ipynb](instrument_classifier.ipynb) jupyter notebook that trains a Deep Convolutional Neural Network and saves the model under folder model.

[demo.ipynb](demo.ipynb) processes a single file by splitting into 1 second parts and producing a mel spectrogram for each one. Then it feeds the mel spectrograms to the trained model in order to identify the instrument playing in each part.
