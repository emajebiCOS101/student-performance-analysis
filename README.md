# student-performance-analysis
DTS 201 group project predicting course pass/fail using student assessment scores.

## Project summary
Our project investigates whether student assessment score can help identify students at risk failing a course.
## Data set
We got the CSV from Mendeley Data: https://data.mendeley.com/datasets/vzfyk22fhn/4
It contains 500 student records and 12 columns. Our original proposal focused on PAU, but we switched to a public dataset, as the required student records were hard to obtain.

We checked for missing values and duplicates, explored assessment
scores and their relationships, and prepared seven assessment
features with a binary outcome: Pass - 0 or Fail - 1. Final examination
marks, total scores, grades and original categories were excluded
from the model inputs.

We compared Logistic Regression and a Decision Tree using five-fold
stratified cross-validation on the training data. The selected
Decision Tree achieved 96.43% accuracy and identified five of eight
actual failures in the test set. The Most-Frequent baseline achieved
92.86% accuracy but identified no failures. We also compared against
a Uniform baseline.

The dataset is imbalanced, and the test set contained only eight
failure cases. Results have not been validated at PAU or other
universities, and predictions are not guaranteed outcomes.

## Repository Contents

- `Students_Performance_Project.ipynb`: Complete workflow, including
  data loading, exploration, preparation, modelling and evaluation.
- `Daniel_Data_Loading.ipynb`: Dataset source and loading.
- `Dara_Exploration.ipynb`: Exploratory analysis and visualisations.
- `Solomon_Data_Preparation.ipynb`: Data checks, feature selection,
  outcome labels and train/test splitting.
- `Eiza_Model_Training.ipynb`: Model comparison, selection and training.
- `Odinaka_Model_Evaluation.ipynb.ipynb`: Baseline comparison and evaluation.
- `Student Performance Dataset 2024.csv`: Original dataset.
- `cleaned_data.csv`: Prepared features and pass/fail label.
- `requirements.txt`: Python libraries required to run the code.
- Presentation PDF: Project findings, results and recommendations.

## How to run the Code
1. Open `Student_Performance_Project.ipynb` in Google Colab.
2. Connect to a runtime.
3. Run all cells in order from top to bottom. The dataset is loaded
   directly from the public GitHub repository, so no manual upload
   is required.

The required libraries are listed in `requirements.txt`

Use the complete notebook to run the full project. Individual
notebooks contain sections that may depend on earlier preparation.

## Group Contributions

- Daniel: Dataset source and loading.
- Dara: Exploratory data analysis and visualisation.
- Solomon: Data preparation and train/test splitting.
- Eiza: Model training, comparison and selection, README file, slides.
- Odinaka: Model evaluation and baseline comparison.
