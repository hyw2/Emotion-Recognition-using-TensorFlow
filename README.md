# Facial-Recognition-using-TensorFlow
### This repository was developed by following the TensorFlow for poets guide on [codelabs](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/?utm_campaign=chrome_series_machinelearning_063016&utm_source=gdev&utm_medium=yt-desc#0). 

It uses two repositories "happy" and "frown" as training data to determine whether a person in the image is smiling or frowning. 

### Requirements:
[Docker](https://www.docker.com/community-edition)

### Usage:
Start the Docker image in terminal using:
```
docker run -it \
  --publish 6006:6006 \
  --volume ${HOME}/tf_files:/tf_files \
  --workdir /tf_files \
  tensorflow/tensorflow:1.1.0 bash
```
then run the python script label_image.py with a jpg image as an argument, i.e.:
```python
python label_image.py photo.jpg
```
