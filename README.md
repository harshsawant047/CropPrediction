# 🌾 Crop Yield Prediction and Recommendation System (India)

This project provides a **Machine Learning-based solution** to predict crop yield and recommend the most suitable crops for different regions of India based on environmental and soil parameters.

---

## 📌 Features

- ✅ Predict crop yield using weather and soil inputs  
- ✅ Recommend crops based on soil health, location, and season  
- ✅ Uses historical Indian agriculture datasets  
- ✅ Implements a complete ML pipeline (preprocessing → training → prediction)  
- ✅ Persist models using `pickle` for deployment  

---

## 🧠 Technologies & ML Models Used

- **Programming Language**: Python  
- **Core Libraries**:  
  - `pandas`, `numpy`  
  - `scikit-learn`  
  - `pickle` for model serialization  
  - `logging` for debugging and traceability  
  - `os` for system-level operations  

- **ML Models**:
  - `RandomForestClassifier`: for crop recommendation
  - `LinearRegression`: for crop yield prediction

- **Preprocessing Tools**:
  - `OneHotEncoder`: to handle categorical features like state, season  
  - `StandardScaler`: to normalize numerical features  
  - `Pipeline` and `ColumnTransformer`: to automate and manage the preprocessing and training pipeline  
  - `train_test_split`: for model evaluation

---

## 🗂️ Dataset Details

- **Sources**:
  - [data.gov.in](https://data.gov.in)
  - [Kaggle Indian Crop Data](https://kaggle.com)
  - IMD Rainfall and Temperature data

- **Fields**:
  - State, District, Season  
  - Rainfall (mm), Temperature (°C)  
  - Soil pH, Nitrogen (N), Phosphorus (P), Potassium (K)  
  - Crop name, Production (kg/hectare)

---

## 🔧 Installation

```bash
git clone https://github.com/yourusername/crop-yield-prediction-india.git
cd crop-yield-prediction-india
pip install -r requirements.txt
```

---

## 🚀 How to Use

### 1. **Train the model** (if not already trained):

```python
python train_model.py
```

This will:
- Load the dataset  
- Apply preprocessing  
- Train both the classifier and regressor  
- Save the trained models using `pickle`

### 2. **Run the app** (if using Streamlit or Flask):

```bash
streamlit run app.py
```

or

```bash
python app.py
```

### 3. **Provide Input**:
- Soil nutrients (N, P, K), pH  
- Rainfall, Temperature  
- Season, Location

### 4. **Output**:
- 🎯 Recommended crops
- 📈 Predicted yield for selected crop (kg/hectare)

---

## 🧪 Example Code Snippet

```python
from sklearn.ensemble import RandomForestClassifier
from sklearn.linear_model import LinearRegression

model = RandomForestClassifier()
regressor = LinearRegression()
```

---

## 📦 Output Files

- `model_classifier.pkl`: Pickled Random Forest Classifier for crop recommendation  
- `model_regressor.pkl`: Pickled Linear Regression model for yield prediction  
- `scaler.pkl`, `encoder.pkl`: Preprocessing transformers  

---

## ✅ Future Enhancements

- Real-time weather data integration  
- Fertilizer recommendations  
- Geo-based auto-detection using GPS  
- Support for regional languages  
- Mobile version for Android

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Authors

- [Your Name](https://github.com/yourusername)  
- Collaborators from [Your Institution Name]
