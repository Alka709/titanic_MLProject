#  Titanic Survival Prediction Project

This project uses the **Titanic dataset** to predict whether a passenger survived or not based on various features such as age, gender, fare, class, and titles derived from names. The goal is to apply feature engineering and train multiple classification models to evaluate their performance.

---

##  Features Used

- **Pclass** (Passenger class)
- **Sex**
- **Age**
- **SibSp** (Siblings/Spouses aboard)
- **Parch** (Parents/Children aboard)
- **Fare**
- **Embarked**
- **FamilySize** = SibSp + Parch + 1
- **Alone** (Whether the passenger was alone or not)
- **Title** (Extracted from the Name column)

---

## ⚙️ Feature Engineering

- **Title extraction** from Name (`Mr`, `Mrs`, `Miss`, etc.)
- Created **FamilySize** and **Alone** features
- Handled missing values (especially for `Age` and `Fare`)
- Encoded categorical features (e.g., `Sex`, `Embarked`, `Title`) using **get_dummies**
- Applied **StandardScaler** to scale features 

---

## 🧠 Models Trained

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**

All models were evaluated using **accuracy score**. Interestingly, all performed with very similar accuracy levels.

---

## 📉 Evaluation

- Accuracy metrics for each model were compared.
- Missing values were handled before model training.
- Scaling was applied only on the feature inputs (`X_train` and `X_test`) **after splitting**.

---

## 🚧 Challenges Faced

- Handling missing values (`Age`, `Fare`) correctly before scaling
- Understanding why feature scaling is important and how it should be applied
- Proper encoding of categorical features for ML models

---

## ✅ Final Thoughts

This beginner-friendly project taught me the complete ML pipeline:
- Cleaning data
- Feature engineering
- Model training & evaluation
- Importance of preprocessing like imputation and scaling

---

## 💻 Tools Used

- Python 🐍
- Pandas, NumPy
- Scikit-learn
- Jupyter Notebook

---

## 📂 How to Run

1. Clone this repo
2. Install the required libraries (e.g. `pip install -r requirements.txt`)
3. Open the `.ipynb` notebook in Jupyter or VS Code
4. Run the cells to train the models and view outputs

---

Made with ❤️ while learning machine learning!
