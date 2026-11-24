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

- `Student_Performance_Project.ipynb`: Complete workflow, including
  data loading, exploration, preparation, modelling and evaluation.
- Individual member notebooks: Each member’s contribution.
- `Student Performance Dataset 2024.csv`: Original dataset.
- `student_performance_cleaned.csv`: Prepared features and pass/fail label.
- `requirements.txt`: Python libraries required to run the code.
- Presentation PDF: Project findings, results and recommendations.

## How to run the Code

1. Open `Student_Performance_Project.ipynb` in Google Colab.
2. Download the original dataset CSV from this repository.
3. Upload it into Colab using the Files panel, keeping its filename
   as `Student Performance Dataset 2024.csv`.
4. The notebook loads it from:
   `/content/Student Performance Dataset 2024.csv`.
5. Run the notebook cells in order from top to bottom.

The required libraries are listed in `requirements.txt`. If any are
unavailable, run this in a Colab code cell:

    %pip install pandas matplotlib seaborn scikit-learn

Use the complete notebook to run the full project. Individual
notebooks contain sections that may depend on earlier preparation.

## Group Contributions

- Daniel: Dataset source and loading.
- Dara: Exploratory data analysis and visualisation.
- Solomon: Data preparation and train/test splitting.
- Eiza: Model training, comparison and selection.
- Odinaka: Model evaluation and baseline comparison.
