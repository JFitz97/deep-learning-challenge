# deep-learning-challenge
For this challenge, I used machine learning to create a tool that will help Alphabet Soup, a non-profit foundation, select funding applicants with the best chance of succeeding in their venture. I created a binary classifier that will predict the fate of a venture based on: 
* Identification number & name of applicant
* Alphabet Soup's application type
* Affliated sector of  inducstry
* Goverment organization classification
* Funding use case
* Organization type
* Active status
* Income classification
* Special considerations taken
* Funding request amount

## Data Pre-processing

To create an accurate model, I had to pre-process some of the raw data. First, the application name and ID number columns werre dropped as they do not provide any value for the model. Then, I binned some of the rarely occuring application type's and governemnt organization classifications into an "other" category. I used "get_dummies" to convert all categorical data into numerical data. I split the raw dataset into Test and Train sets, and scaled the data using StandardScaler. 

## Compile, Train, and Evaluate Model
I used TensorFlow and Keras to make a neural network with two hidden layers and an output layer. I compiled the model and trained it with 30-100 epochs. The highest accuracy score I achieved was 74%. 


## Optimize
I used various tactics in attempt to optimize the model. I tried changing the number of hidden layers, as well as the units and activation method of each layer. I tried compiling the model with different optimizers, and also varied the number of epochs used to train the model. Ultimately, none of this resulted in a model with 75%+ accuracy, which leads me to believe that I would need to do additional data cleaning/pre-processing to achieve these results. 
