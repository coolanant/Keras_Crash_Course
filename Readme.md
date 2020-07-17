## Installation

python+anaconda+pycharm+keras+tensorflow

activate keras
pip install tensorflow

pycharm -> create project -> interpreter -> conda ->3.5

anaconda prompt ->
conda create -n (keras)
activate keras
pip install tensorflow
conda install -c conda-forge keras
conda install -c conda-forge google-api-python-client

## Basics

keras - frontend
tensorflow - backend

1. Choose Model (Supervise learning model)
2. Training
3. testing
4. Evaluation

OR Colab.Google.com

## Tips

1. Default are best practices
2. Neural Networks work best if data in each col is all scaled to same range (for ex. 0 to 1)
3. tensor Board

## Example

### Defining Model

model=kears.models.Sequential()
model.add(kera.layers.Dende(32,input_dim=9))
model.add(kera.layers.Dende(128,activation=")) //128 ndoes/optic nerve
model.compile(loss='adam',optimizer='mse')

### Training Phase

model.fit(training_data,expected_output)

### test

error_rate=model.evaluate(testing_data,expected_output)

model.save("--.h5")

### Evaluation Phase

model=keras.models.load_model("--.h5")
predictions=model.predict(new_data)

## LAYERS

1. Dense
2. convolutional.Conv2D() -images/spatial data
3. recurrent.LSTM()

---

### Export your model to gcloud

Google Cloud
Google CLoud Machine Learning -> machine Learning Engine Api
cloud.google.com/sdk/downloads ->interactive installer
gcloud init
