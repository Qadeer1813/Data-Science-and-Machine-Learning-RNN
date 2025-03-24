# Data-Science-and-Machine-Learning-RNN

**Student Name: Qadeer Hussain**

**Student ID: C00270632**

**Lecture: Greg Doyle**

**Lecture: Recurrent Neural Networks (RNN)**

# Disclaimer 
**This project is intended for educational purposes only.
It was developed to explore Recurrent Neural Networks (RNNs) and natural language generation.No part of this project is intended for commercial use or to infringe upon any copyrights**

# Project Description
The purpose of this project is to train a Recurrent Neural Network (RNN) using LSTM layers to generate poetry-like text character-by-character. The model learns the structure, style, and patterns of Emily Dickinson’s poems by analyzing the sequence of characters within them.

# Data Source
The dataset that was used for this project can be downloaded from https://www.gutenberg.org/ebooks/1057

# Processing
After downloading this dataset, a test print was conducted ```print("Total Characters in Raw Text:", len(raw_data))```, ```print(raw_data[:1000])```. The loaded data is then displayed. Since the poems begin from line 209, the following line of code was used ```poem_lines = raw_data[209:]```. To clean the data blank lines, lines written in all-uppercase, and lines containing only numbers were removed, ensuring only the actual poem content was kept for training. Joined all the poem lines into one continuous string and converted it to lowercase to maintain consistency. Finally, all unique characters were extracted from the text and created mappings to convert characters to numerical indices. After cleaning was done, the cleaned text was split into sequences of 100 characters to prepare training data. These sequences were then converted to numbers and one-hot encoded so the model could learn patterns and predict the next character. After this, the model was built. The model was then trained over 20 epochs with a batch size of 256. During training, both the accuracy and loss were tracked and visualized using matplot library. Finally, the model was tested by generating text based on a seed phrase at different temperature values to explore how randomness affects the output.

# Data Understanding and Visualisation 
After the data was processed and the model was built, trained and tested these were the following results:

1. Training loss

   ![image](https://github.com/user-attachments/assets/bb24f823-2eeb-4ad8-b969-da5c9c5f3722)

2. Training Accuracy

   ![image](https://github.com/user-attachments/assets/34ebb838-7c2f-449b-b336-0ceee60a6886)

3. Model in use

   ![image](https://github.com/user-attachments/assets/cef88c69-2e44-4ee6-a43d-75c6ba290abc)

# Algorithims:
Recurrent Neural Networks: RNNs are a type of neural network designed for sequential data. They maintain memory of previous inputs, making them ideal for tasks like text generation. In this project, an RNN with LSTM layers was used to learn and generate poetry character by character.

# Online Sources:
1. Trekhleb (2025) Trekhleb/machine-learning-experiments: 🤖 interactive machine learning experiments: 🏋️models training + 🎨models demo, GitHub. Available at: https://github.com/trekhleb/machine-learning-experiments (Accessed: March 2025). 
2. User guide# (2025) User Guide - pandas 2.2.3 documentation. Available at: https://pandas.pydata.org/docs/user_guide/index.html (Accessed: March 2025).
3. Matplotlib 3.9.2 documentation# (2025) Matplotlib documentation - Matplotlib 3.9.2 documentation. Available at: https://matplotlib.org/stable/ (Accessed: March 2025).
4. Tensorflow (2025) TensorFlow. Available at: https://www.tensorflow.org/ (Accessed: March 2025). 

# Tools and Tech Used: 
1. Recurrent Neural Networks
2. Jupter Notebook
3. Pandas Library - Loading the data and analysing it
4. Matplotlib - Plotting and Visualising the graph 
5. Tensorflow
6. Numpy
