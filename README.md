# Thyroid-Disease-Detection
# Problem Statement:
Thyroid disease is a common cause of medical diagnosis and prediction, with an onset 
that is difficult to forecast in medical research. The thyroid gland is one of our body's 
most vital organs. Thyroid hormone releases are responsible for metabolic regulation. 
Hyperthyroidism and hypothyroidism are one of the two common diseases of the thyroid 
that releases thyroid hormones in regulating the rate of body's metabolism.  
The main goal is to predict the estimated risk on a patient's chance of obtaining thyroid 
disease or not.

# Data used

Get the data from https://archive-beta.ics.uci.edu/dataset/102/thyroid+disease  
Quinlan,Ross. (1987). Thyroid Disease. UCI Machine Learning Repository. https://doi.org/10.24432/C5D010.


## Run Locally

Clone the project

```bash
    git clone https://github.com/shivamshinde123/Thyroid_Disease_Detection_Internship.git
```

Go to the project directory (let's say Thyroid-disease-detection)

```bash
    cd Thyroid-disease-detection
```

Create a conda environment

```bash
    conda create -n environment_name python=3.10
```

Activate the created conda environment

```bash
    conda activate environment_name
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Load the data

```bash
  python src/step1_make_dataset.py
```
Validate the loaded data

```bash
  python src/step2_training_Data_Validation.py
```
Preprocess the validated data

```bash
  python src/step3_data_preprocessing_stage1.py
```
```bash
  python src/step4_data_preprocessing_stage2.py
```
Training a machine learning model using preprocessed data and also evluating metrics

```bash
  python src/step5_model_training.py
```
Visualize the metrics in different experiments

```bash
  mlflow ui
```
Testing the code for
 - Data Loading
 - Data Validation
 - Data Preprocessing
 - Model Training and Evaluation

```bash
  pytest src/
```

Make predictions using trained model

```bash
  streamlit run src/webapp.py
```

## 🚀 About Me
I'm an aspiring data scientist and a data analyst.

