# [Brain Tumor Detection](https://github.com/0raghad/Brain-Tumor-Detection-)

  used tools: python, matplotlib, NumPy, TensorFlow, Keras.
  
## Goals and Motivation:

   - assist radiologists and doctors in making accurate diagnoses and treatment plans.
   - Based upon this concept, a user can take a photo and access information about brine tumors by using an application.
   
## Dataset Exploration:  

   - After loading both the dataset using the TensorFlow load dataset method, the following conclusions are drawn:
   - There are 2 brain categories.
   - There are 253 brain images.
   - They are in total 155 healthy brain images. no –> healthy
   - They are in total 98 with tumors brain images. yes –> there are tumors
   
## Visualization:

      Here is a sample of the data:
   
   ![Screenshot (649)](https://user-images.githubusercontent.com/80716758/160547946-bfec54d3-5234-4101-9290-a7461af2a257.png)
     
## Before building model activates:

   1- prepper the train test split in TensorFlow:
      80% of the data will be for training
      then 20% of the data will be separated to 10% for validation at the end of each EPOCHS, 10% for testing.
   2- images preprocessing:
      - resize and rescale the images
      - augmentation 
      
## Modeling:

      built the model using Sequential
      
## Results:

      Below is an example of a prediction using the final model
  ![Screenshot (650)](https://user-images.githubusercontent.com/80716758/160552879-764fa9de-5496-447e-b0be-4a50b16c3e71.png)
  
  
  
# [Customer churn prediction](https://github.com/0raghad/churn)

   used tools: Python, Pandas, NumPy, Matplotlib
   
## Goals and Motivation:
   
     - Testing out several different models to see how they will perform this task.
     - Help companies improve their Customer Retention Strategies by analyzing customer behavio
     
## Dataset Exploration: 
   
    - After loading the dataset the following conclusions are drawn:
    - 21 features and 7043 rows.
    - Dataset mostly has categorical variables that need to be encodeing to numerical variables.
    - the target column is `Churn` 1 will indicates a churned customer 0 otherwise.
    
## Visualization:
   
 ![Screenshot (935)](https://user-images.githubusercontent.com/80716758/167172391-bd9c1942-210d-4c44-8914-2b85cee552e2.png) 
 ![Screenshot (936)](https://user-images.githubusercontent.com/80716758/167172835-2d25f859-38c4-4ed6-bd48-748d130d36f6.png)
 ![Screenshot (941)](https://user-images.githubusercontent.com/80716758/167174329-85cc9e48-dbfe-4bcc-94d9-d10c036a32ba.png) 
 ![Screenshot (942)](https://user-images.githubusercontent.com/80716758/167176439-3d4238f9-25ea-4eaf-9559-d64e142b1397.png)
 
 
###  As seen in the above images, we should focus our efforts on customers who fit the following criteria:
   
    - Internet service: Fiber optic
    - Payment method: Electronic check
    - Contract type: Month-to-month
    - Tenure: Short-term Tenure
    
## Before building model activates:
   
    - Encode the categorical variables. 
    - deal with any missing value that may result after the Encodeing process.
    - deop highly Correlated Columns.
    - train test split the data into 20% for testing and 80% training.
    
## Modeling:
   
     bulit 6 diffrent model to test them:
     LogisticRegression, KNN, SVC, DecisionTree, Random_Forest, XGBoost.
     the models were evaluated using :
     ROC AUC, precision, Recall,F1 score.
     
 ![Screenshot (944)](https://user-images.githubusercontent.com/80716758/167205417-ec59c392-8302-478b-b221-c3dc7519e831.png)
  
   Finally,after ploting the ROC curves of each model with their corresponding Area Under the Curve (AUC). The Area Under the Curve measures the performance of the    model across all possible thresholds for classification. With a higher AUC, a model is capable of better distinguishing between classes.   
   **XGBoost** performs better than the other models.
      
    
# [Toxic Comment Classification](https://github.com/0raghad/toxic_comments)

 used tools:  python, matplotlib, NumPy, pandas, TensorFlow, gradio
 
## Goals and Motivation:
   
      - Develope an artificial intelligence system that detects different types of toxicity in comments using natural language.
      - Aim to prevent toxic comments from showing up
      
      
## Before building model activates:
   
      - sprate the data into target and features
      - vectorizer using TextVectorization
      - create TensorFlow dataset pipeline
      - train test and validation split the data into 10% for testing and 70% for training and 20% for validation
      
      
## Modeling:
   
      built the model using Sequential
      
## Results:
   
       finally here is a snippet of the gradio app 
       
   ![Screenshot (945)](https://user-images.githubusercontent.com/80716758/167214889-7cd96f13-d816-4b52-8f2b-b33df2fb3d8e.png)

       
