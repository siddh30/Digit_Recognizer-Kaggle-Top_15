#  <p align = 'center'> Digit_Recognizer-Kaggle_Competion 
<p align = 'center'> Hit Top 15% in an unranked Kaggle competition with an accuracy of 0.9946 </p>


<p align = 'center'> <img width="1500" img height= "400" alt="submission" src="https://github.com/siddh30/Digit_Recognizer-Kaggle_Competion/blob/main/Leaderboard-2022.png"> </p>

### Objective
To classify handwritten digits from 0-9 as labels (classes) - [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

### Data
<img width="110" img height= "210" alt="submission" src="https://github.com/siddh30/Digit_Recognizer-Kaggle_Competion/blob/main/data.png"> 
- Train : A csv of 784 features - Each feature being a pixel value for a 28*28 image. A target feature containing labels
- Test : A csv of 784 features - Each feature being a pixel value for a 28*28 image
- Sample Sumbission Csv - A sample submission file telling us how the submission file should look like

### Approach
Built a custom CNN model which had the following architecture

<img width="400" img height= "1200" alt="submission" src="https://github.com/siddh30/Digit_Recognizer-Kaggle_Competion/blob/main/model_plot.png"> 

### Tips thats really helped:

- Adding More Layers (Making the Network deeper to decrease training loss)
- Including Batch Norm, Max Pooling, Padding Layers
- Experimenting with different values of Dropout Regularization (Decreasing Validation Loss and hence reduce overfitting)
- Experimenting with different bacth sizes (64 works best)
- Setting up Callbacks : -
  1. Learning Rate Scheduler to slow down learning as the model reached Convergence Point
  2. Saving and Loading from best model with the focus on least validation loss
- Finally Ensembling results from various model runs to give a best aggregate results (Mode of prediction labels)




  
