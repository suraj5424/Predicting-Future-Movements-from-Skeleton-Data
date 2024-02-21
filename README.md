### Predicting Future Movements from Skeleton Data


**Skeleton Data Analysis:**
Skeleton data analysis offers valuable insights into human movements and actions, facilitating applications such as fall detection and gesture recognition. This notebook tackles the challenge of predicting future movements based on past skeleton data, leveraging machine learning techniques. The dataset consists of time series of 3D skeleton data collected from individuals performing various activities.

**Imported and Extracted the Data:**
- Installed the Kaggle library and mounted Google Drive to access data.
- Used the Kaggle API to download the dataset and unzipped it.

**Added Necessary Libraries:**
- Imported essential libraries including Pandas, NumPy, Matplotlib, and Torch for data manipulation, visualization, and deep learning.

**Loading the Dataset:**
- Loaded the dataset containing 3D skeleton data from the provided directory.

**Data Preprocessing:**
- Preprocessed the data by selecting relevant columns and handling missing values.
- Transformed the data into a suitable format for further processing.

**Train-Test Split:**
- Split the data into training and testing sets for model evaluation.

**Creating Windows:**
- Created windows of fixed size from the time series data for sequential processing.
- Generated corresponding labels for the windows.

**Converted Windows into Tensors:**
- Converted the windowed data into PyTorch tensors for compatibility with deep learning models.
- Prepared the data for model training and evaluation.

**Selected Available Device:**
- Utilized GPU if available for faster model training.

**CNN One-Dimensional Architecture:**
- Defined a one-dimensional convolutional neural network (CNN) model tailored for sequential data.
- Configured the CNN layers and fully connected layers for feature extraction and classification.

**Training the Model:**
- Trained the CNN model using cross-entropy loss and Adam optimizer.
- Monitored the training loss to track model performance.

**Validation of the Model:**
- Evaluated the trained model on the validation set to assess its accuracy.

**Kaggle Predictions:**
- Utilized the trained model to make predictions on the test set.
- Generated submission file containing the predicted labels for each signal.

**Writing the Solution in Submission File:**
- Created a submission file in CSV format containing the predicted labels for each signal in the test set.

This notebook provides a comprehensive approach to predicting future movements from skeleton data, encompassing data preprocessing, model development, evaluation, and submission formatting. By leveraging deep learning techniques, we aim to develop an accurate predictive model with practical applications in various domains.
