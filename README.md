# Naive Bayes Classifier for Essay Detection

## Instructions to Train and Test the Model on Colab Notebook

1. Upload the dataset files to the Colab session.

2. Replace the file paths in the first cell with the paths to your own dataset files.

3. Replace the Hugging Face login token with your own token.

4. Run the cells to train the classifier.

## Predicting the Class of a Sample Essay

To predict the class of a sample essay, use the `predictClass` method.

Example usage:

```python
# Instantiate the classifier (ensure it's already trained)
classifier = NaiveBayes(your_train_data)

"your_train_data" : it should be a pandas dataframe with two necessary attibutes with exact same names,
 'text'; which is the essay and the other is class label with name "genrated", with int value 0 denoting
 human generated and 1 denoting ai generated.

# Provide a sample essay
essay = "Your test essay goes here/n."

# Predict the class
predicted_class = classifier.predictClass(essay)

# Print the result
print(f'The predicted class for the essay is {predicted_class}')
