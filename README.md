# Iris Data Set Assignment 

The Iris flower has two species, Iris-setosa and Iris-versicolor.
Go to Iris Flower Dataset | Kaggle and download the dataset.
Create a model that can predict which species it is based on its features.
Do this in a Jupyter notebook and submit it together with your dataset.

# Requirement
Anaconda
Jupytor

# Installation
## Objective

The Iris dataset consists of 50 samples for each of three species of Iris flower - Iris setosa, Iris virginica, and Iris versicolor. Each sample is comprised of 4 measurements or features - sepal length, sepal width, petal length, and petal width. Our objective was to Create a model that can predict which species it is based on its features.

# Loading the Data
Go to Iris Flower Dataset https://www.kaggle.com/datasets/arshid/iris-flower-dataset Kaggle and download the dataset.
Upload it to your Jupyter notebook and read the file with this code
df = pd.read_csv("IRIS.csv")
print(df.head(4))

# Training the DataSet
Code can be found at https://github.com/SarfoEmmanuel/Irisassignment/blob/main/irisfinalassgnment.ipynb


# Final Remarks
##Predicting the species

# Tying out the model with the feature input: [sepal_length, sepal_width, petal_length, petal_width]
new_sample = np.array([[5.1, 3.5, 1.4, 0.2]]) 

# Predicting species (returns a numerical value)
predicted_label = model.predict(new_sample)
visualize it to predict what should be achieved by the model

# Ploting the features
plt.figure(figsize=(6, 4))
plt.bar(["Sepal Length", "Sepal Width", "Petal Length", "Petal Width"], new_sample[0], color=['red', 'blue', 'green', 'orange'])
plt.xlabel("Features")
plt.ylabel("Measurement (cm)")
plt.title("Flower Feature Measurements")
plt.show()

# Predicting species (returns a numerical value)
predicted_label = model.predict(new_sample)

# Converting numeric prediction back to species name
predicted_species = le.inverse_transform([int(round(predicted_label[0]))])

print(f"Predicted Species: {predicted_species[0]}")

# Predicted Species: Iris-setosa

# Enjoy

