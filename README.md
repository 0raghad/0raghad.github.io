# Brain Tumor Detection
  used tools: python, matplotlib, NumPy, TensorFlow, Keras.
  
  Goals and Motivation:
   - assist radiologists and doctors in making accurate diagnoses and treatment plans.
   - Based upon this concept, a user can take a photo and access information about brine tumors by using an application.
  Dataset Exploration:  
   - After loading both the dataset using the TensorFlow load dataset method, the following conclusions are drawn:
   - There are 2 brain categories.
   - There are 253 brain images.
   - They are in total 155 healthy brain images. no –> healthy
   - They are in total 98 with tumors brain images. yes –> there are tumors
  Visualization:
   Here is a sample of the data:
     ![Screenshot (649)](https://user-images.githubusercontent.com/80716758/160547946-bfec54d3-5234-4101-9290-a7461af2a257.png)
  Before building model activates
   1- prepper the train test split in TensorFlow:
      80% of the data will be for training
      then 20% of the data will be separated to 10% for validation at the end of each EPOCHS, 10% for testing.
   2- images preprocessing:
      - resize and rescale the images
      - augmentation
  Modeling:
      built the model using keras.models.Sequential
  Results:
      Below is an example of a prediction using the final model
   ![Screenshot (650)](https://user-images.githubusercontent.com/80716758/160552879-764fa9de-5496-447e-b0be-4a50b16c3e71.png)

