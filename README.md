Plantright is a data mining project developed as part of the Application of Data Mining in Public Sector assignment at General Sir John Kotelawala Defence University (Intake 41). The project aims to assist farmers and policymakers by recommending the most suitable crops based on soil nutrients and climatic conditions using machine learning methods. Problem Statement

Selecting the best crop based on soil and weather conditions remains a major challenge for farmers. This project addresses the research question:

“How can we accurately predict the most suitable crop for cultivation based on soil composition and environmental conditions?”

Through data-driven insights, Plantright supports:

Improved farm-level decision-making

Better resource optimization

Promotion of sustainable agriculture

## Dataset ##

Dataset Name: Crop Recommendation Dataset Source: Figshare (ICFA & ICAR collaboration)

Records: 2,200 Features: 7 independent + 1 dependent (crop type)

Feature Description N Nitrogen content in soil P Phosphorus content K Potassium level Temperature (°C) Temperature of environment Humidity (%) Relative humidity pH Soil acidity/alkalinity Rainfall (mm) Total rainfall Crop Type Target variable — suitable crop label ⚙️ Methodology

Data Preparation
Loaded and cleaned dataset using R

Checked for missing values (none found)

Standardized numerical features using Z-score normalization

Split data into 70% training and 30% testing

Data Mining Technique: K-Nearest Neighbors (KNN)
KNN selected for classification due to simplicity and interpretability

Optimal K value found through Error Rate vs. K plot

Evaluated model using confusion matrix and performance metrics

📈 Results and Model Performance Metric Result Accuracy 96% Precision 97.66% Recall 97.27% F1-Score 97.46%

✅ The model demonstrates strong reliability and consistency in predicting the best crop for given soil and climate conditions. ✅ Low error rate achieved for K = 5. ✅ Visual analyses confirm good classification balance and minimal misclassification.

🌾 Impact 🔹 Agricultural Decision Support

Provides farmers with evidence-based crop recommendations.

🔹 Resource Optimization

Efficient water, fertilizer, and equipment use.

🔹 Environmental Sustainability

Encourages biodiversity, reduces pollution, and supports climate-resilient farming.

🔹 Policy & Economic Benefits

Assists policymakers with agricultural planning, improves yield, and reduces cost for farmers.

## Key Learnings ##

Data mining can effectively improve agricultural decision-making.

KNN delivers high accuracy for crop classification using soil and climate variables.

Evidence-based systems can significantly enhance sustainability and productivity in agriculture.

Implementation Details

Language: R Key Libraries:

caret – Model training & data partitioning

class – KNN implementation

ggplot2 – Data visualization

dplyr – Data cleaning & transformation
