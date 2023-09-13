# Prediction & Optimisation of Furnace Operations through data analytics & deep learning
Study and predication of the Coil pressure ratio at GAIL PATA
petrochemical Plant with the help of deep learning LSTM techniques

# Understanding the Model - LSTM
• Long Short Term Memory (LSTM) networks are a type of recurrent neural network capable of learning order dependence in sequence prediction problems  

• These networks are capable of capturing the dynamicity of the data, hence are suited best for forecasting purposes. They work tremendously well on a large variety of problems, and are now widely used.

• These networks are capable of capturing the dynamicity of the data, hence are suited best for forecasting purposes

• LSTMs have a chain like structure, having a repeating module as depicted in the figure on previous slide. There are four layers inside of a module, interacting in a very special way.

# About Results
The dataset ranges from February 2018 to November 2021. In order to encompass all the possible scenarios, data recorded during shutdowns has also been included. The sampling frequency is 10 minutes, hence 1,56,405 samples in total. Till date, data collection is still on

after initial preprocessing, the total no. of samples for model development = 1,38,277 with 11 different attributes

# Since not all data can be fed to an algorithm at once, some preprocessing had to be done. This included

• Removal of samples where dry feed flow wasn't there at occurrences of plant shutdown.

• Instances when instruments were taken off line for maintenance have been discarded from the history.

# Model Architecture

•Size of input window = 144

•Size of output window = 6

•Train - Test - Validation split = 70:10:20

•Total no. of batches of train data = Train size/(a+b)

•Optimizer used = Adam

•Learning rate = 0.001/0.002

•No. of LSTM units = Dependant upon no. of batches

# Train Loss v/s Validation Loss

Though near ideal condition of training and validation losses converging close to zero is being achieved, but further improvements can be done.
