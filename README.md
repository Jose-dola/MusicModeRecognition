# MusicModeRecognition
Deep Learning model to recognize music mode of audio samples. The future aim of this project is to recognize not only the music mode but also the key.
The code consists of three jupyter notebooks:
- generating_dataframe_with_key_mode_and_corresponding_files.ipynb: To label the data, this notebook matches audio files (songs) with the corresponding rows in a pandas dataframe that has information about the songs (e.g. the mode).
- generating_spectogram_and_labels_data_for_feeding_the_neuralNet.ipynb: This notebook unifies audio signals -sampling rate and bitrate-, frames the audio signals, applies Short Time Fourier Series, filters the resulting STFS, and, finally, makes the Spectograms that will feed the model.
- building_neuralNet_for_song_mode_detection.ipynb: In this notebook a Deep Learning model is built and trained using the Spectogram data and labels generated in the previous notebook.
