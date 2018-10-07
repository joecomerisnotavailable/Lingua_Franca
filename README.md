# What:
A convolutional neural network for recognizing the language being spoken in short (about 3-10 second) wav recordings by first converting the raw audio to Mel-Frequency Cepstral Coefficient images.

# How:
To train: Run `train.py --modeldir=[directory_to_save_model] <-v[erbose_logging]>`

To test: Drop any desired test audio into the test-audio folder, add the filename and label to the files.csv file there, and run `predict.py --modeldir=[directory_of_saved_model] <-v[erbose_logging]>

# Requirements:
argparse
tempfile
tensorflow >1.8.0
numpy
pandas
sklearn