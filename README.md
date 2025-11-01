# Obesity Levels Prediction

##  Project Overview  
This project aims to predict individuals’ obesity levels using lifestyle and health-related features. I applied data preprocessing, feature engineering, and built classification models (Decision Tree & Logistic Regression) to classify obesity into multiple levels based on the dataset.

##  Dataset  
The dataset includes various features such as eating habits (e.g., frequent high-calorie food consumption), transportation mode, family history of overweight, and demographic information. The target variable is **“NObeyesdad”**, which indicates the class of obesity (e.g., Normal Weight, Overweight Level I/II, Obesity Type I/II/III).

##  Data Preprocessing & Feature Engineering  
- Cleaned and standardized categorical variables (e.g., gender, smoking status).  
- Converted categorical features to binary/one-hot encodings where appropriate (e.g., `MTRANS_Walking`).  
- Excluded features that showed minimal distinction across target classes (e.g., `SMOKE`, `SCC`).  
- Balanced class distributions and prepared inputs for classification modeling.

##  Models Used  
- **Logistic Regression** – baseline classifier for multiclass obesity prediction.  
- **Decision Tree Classifier** – used to capture non-linear relationships and feature interactions more effectively.
- **K-Nearest Neighbors (KNN)** - Distance-based lazy learning method
- **Support Vector Machine (SVM)** - Kernel-based high-dimensional classifier
- **Naive Bayes (GaussianNB)** - Probabilistic model assuming feature independence

##  Results & Evaluation  
Among all tested algorithms, the models achieved strong performance, with Decision Tree and SVM yielding the highest accuracy %96 on the test data.
Visual evaluation of confusion matrices confirmed effective class separation for most obesity categories.

##  Insights & Conclusion  
- Regular physical activity (e.g., walking) and dietary patterns play a key role in obesity risk.  
- Excluding less informative features simplifies the model and maintains performance.  
- Further model tuning or use of external datasets could improve generalization and robustness.

##  How to Run the Project  
1-Clone the repository:
  git clone https://github.com/emreyoruk64/obesity-levels-prediction.git
  cd obesity-levels-prediction

2-Install the dependencies:
  pip install -r requirements.txt

3-Run the notebook:
  jupyter notebook ObesityLevels.ipynb

##  Technologies Used

Python 3.12

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn (for ML models and metrics)

Jupyter Notebook

 ## License

This project is open-source and available under the MIT License.
