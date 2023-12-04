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

# Provide a sample essay
essay = "Your test essay goes here."

# Predict the class
predicted_class = classifier.predictClass(essay)

# Print the result
print(f'The predicted class for the essay is {predicted_class}')
