# biof509-finalproj
Decision tree classification of autism screening data
Welcome to the BIOF 509 Final Project!  
To begin, first create an instance of the Preprocessing class, found in the project data.ipynb notebook.
If you cannot view the notebook on Github, please use "https://nbviewer.jupyter.org/" and input the Github link to the notebook in order to visualize it.
To initialize your instance of the class, use your dataset (I used the one found here: https://www.kaggle.com/faizunnabi/autism-screening) as the 'raw_data' argument.
Make sure you have either specified the path to the file or that the file is in your current working directory. 
For the 'nanvalues' argument for creating an instance of the Preprocessing class, specify what values in the dataset will be converted to NaN values (example: '?').
If you will drop columns of your dataset, use a list of the column names you want to drop for the 'dropc' argument.
If you will drop rows of your dataset, specify the row numbers you want to drop for the 'dropr' argument.
If you have columns you want to rename in the dataset, create a dictionary in the following fashion: {'original_name':'new_name', etc} for the 'rename' argument.
You have now initialized your Preprocessing class!

For the LabelEncode method of the Preprocessing class, assign '[whatever your Preprocessing class object name is].LabelEncode(data,cols)' to a new variable, say 'LabelEncoded'.
For the 'data' argument of the LabelEncode method, use '[whatever your Preprocessing class object name is].data'.
For the 'cols' argument of the LabelEncode method, use ONE column name, surrounded by brackets (example: ['Class/ASD']).
Then print your new variable to see the label-encoded result!

For the encode method of the Preprocessing class, assign '[Preprocessing class object name].encode(data, cols)' to a new variable, say 'encoded'.
For the 'data' argument of the encode method, use whatever variable you assigned the label encoded data to (example: LabelEncoded , from above).
For the 'cols' argument of the encode method, use a list of column names in the dataset that you want to one-hot encode.
Then print your new variable to see the one-hot encoded result!

For the normalize method of the Preprocessing class, assign '[Preprocessing class object name].normalize(data, cols)' to a new variable, say 'normalized'.
For the 'data' argument of the normalize method, use whatever variable you assigned the one-hot encoded data to (example: encoded , from above).
For the 'cols' argument of the normalize method, use a list of column names in the dataset that you want to normalize.
Then print your new variable to see the normalized result!

Now your data is fully preprocessed.

Now, you need to create an instance of the next class, the Decision_tree class.
To initialize your instance of the Decision_tree class, use whatever variable name you used to create the fully preprocessed dataset (example: 'normalized') as the 'dataset' argument.
For the 'labelsplit' argument, type the name of the column you want as the label column of your dataset, surrounded by brackets (example: ['Class/ASD']).

For the 'results' method of the Decision_tree class, no arguments are needed.  Just type '[Decision_tree class object name].results()' and execute the cell to view the results!

That's it for the project! Thanks for interacting with the code.
