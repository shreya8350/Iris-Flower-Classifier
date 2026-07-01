🌸 **Iris Flower Classifier**

A machine learning web application built with Streamlit and Scikit-learn that predicts the species of an Iris flower based on its physical measurements. The app uses a Random Forest Classifier trained on the classic Iris dataset and provides real-time predictions with confidence scores.

**Project Overview :**

    The Iris Flower Classifier is an interactive web application where users input four physical measurements of an Iris flower and the app instantly predicts its species. The prediction is powered by a Random Forest Classifier trained on the classic Iris dataset. The app also displays confidence scores for each species so the user can see how certain the model is.

**Features :**
- Interactive sliders to enter flower measurements
- Real-time species prediction using a trained ML model
- Confidence score bars for all three species
- Sidebar with model information (type, accuracy, features, classes)
- Option to switch between joblib and pickle model formats

**Dataset :**
      The app uses the Iris Dataset, it is one of the most well-known datasets in machine learning.
----------------------------------------------------      
| Property       | Details                         |
|----------------|---------------------------------|
| Total Samples  | 150 (50 per class)              |
| Features       | 4                               |
| Classes        | 3                               |
| Missing Values | None                            |
----------------------------------------------------

**Input Features :**
---------------------------------------------------
| Feature      | Description               | Unit |
|--------------|---------------------------|------|
| Sepal Length | Length of the sepal       | cm   |
| Sepal Width  | Width of the sepal        | cm   |
| Petal Length | Length of the petal       | cm   |
| Petal Width  | Width of the petal        | cm   |
---------------------------------------------------

**Target Classes :**
----------------------------
| Label | Species          |
|-------|------------------|
| 0     | Iris Setosa      |
| 1     | Iris Versicolor  |
| 2     | Iris Virginica   |
----------------------------

**Machine Learning Model :**
-------------------------------------------------
| Property         | Details                    |
|------------------|----------------------------|
| Algorithm        | Random Forest Classifier   |
| Number of Trees  | 100                        |
| Train/Test Split | 80% / 20%                  |
| Random State     | 42                         |
| Accuracy         | ~96% to 100%               |
| Saved Formats    | joblib and pickle          |
-------------------------------------------------

## Project Structure

```
WEB APP/
├── models/
│   ├── streamlit_app.py        # Main Streamlit application
│   ├── iris_model.joblib       # Trained model in joblib format
│   ├── iris_model.pickle       # Trained model in pickle format
│   ├── model_info.json         # Model metadata
│   └── feature_ranges.json     # Slider range values
├── train_model.py              # Script to train and save the model
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
```

---

Technologies Used :
-------------------------------------------------
| Technology   | Purpose                        |
|--------------|--------------------------------|
| Python       | Core programming language      |
| Streamlit    | Web application framework      |
| Scikit-learn | Training the ML model          |
| NumPy        | Numerical computation          |
| Pandas       | Data display in tables         |
| Joblib       | Saving and loading the model   |
-------------------------------------------------

Installation :

**Step 1 — Create and activate a virtual environment:**
```
python -m venv vname
vname\Scripts\activate
```

**Step 2 — Install required libraries:**
```
pip install -r requirements.txt
```

**Step 3 — Train and save the model:**
```
python train_model.py
```

**Step 4 — Run the app:**
```
streamlit run models\streamlit_app.py
```

**Step 5 — Open in browser:**
```
http://localhost:8501
```
**Live Demo :**
https://iris-flower-classifier-shreya8350.streamlit.app/

**License :**
This project is built for educational and demonstration purposes. The Iris dataset is publicly available and in the public domain.
