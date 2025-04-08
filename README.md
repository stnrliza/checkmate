# CheckMATE Learning Path Documentation  

**CheckMATE** is an innovative machine learning application designed to enhance school environments. With features such as smart attendance tracking, school attribute detection, and mood tracking, CheckMATE supports teachers and parents in monitoring student discipline effectively.  

## Key Features  
- **Attendance Tracking**: Recognizes student faces for automated attendance.  
- **School Attribute Checker**: Ensures students wear proper school attire, such as ties.  
- **Mood Tracking**: Monitors student facial expressions to understand their moods.  

## Models Used  
CheckMATE is powered by three CNN-based machine learning models:  

1. **Attendance Model**  
   - Model: `TF100.keras`  
   - Categories: 4 classes (Liza, Nabila, Zain, NoFace)  
   - Algorithm: Transfer learning with MobileNetV2, fine-tuned on the final layers.  
   - Dataset: Custom-made with balanced photos across all classes.  

2. **School Attribute Model**  
   - Model: `dasidasi.keras`  
   - Categories: 2 classes (Wearing a Tie, Not Wearing a Tie)  
   - Algorithm: Transfer learning with MobileNetV2, retrained on all layers.  
   - Dataset: Custom-made with balanced photos for each class.  

3. **Mood Tracker Model**  
   - Model: `ekspresi.keras`  
   - Categories: 4 expressions (Happy, Sad, Neutral, Angry)  
   - Algorithm: A simple CNN without a pre-trained model.  
   - Dataset: FER2013 from Kaggle (converted from 7 expressions to 4).  

## Development Process  
- **Dataset Preparation**: Collected custom photos and cleaned the data to ensure quality.  
- **Data Augmentation**: Applied augmentation techniques to expand the dataset.  
- **Model Training**: Trained the models with transfer learning and evaluated them using a confusion matrix.  
- **Optimization**: Utilized regularization, dropout, and a flatten layer to improve model performance.  

## Advantages  
- **Efficiency**: Powered by cloud technology to save resources.  
- **Accuracy**: Well-trained models deliver reliable results for student and school attribute detection.  
- **User-Friendly**: Designed for seamless integration into everyday school activities.  

We hope CheckMATE becomes a practical solution for improving student discipline and streamlining school management. Let’s create a better learning environment with CheckMATE!  
