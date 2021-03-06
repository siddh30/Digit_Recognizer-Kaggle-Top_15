#  <p align = 'center'> Digit Recognizer </p>
<p align = 'center'> Hit top 15% in an unranked Kaggle competition with a score of 0.9946 </p>



<p align = 'center'> <img width="1500" img height= "400" alt="submission" src="https://github.com/siddh30/Digit_Recognizer-Kaggle_Competion/blob/main/Leaderboard-2022.png"> </p>

## Objective
To classify handwritten digits from 0-9 as labels (classes) - [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

### Data
<img width="410" img height= "200" alt="submission" src="https://github.com/siddh30/Digit_Recognizer-Kaggle_Competion/blob/main/data.png"> 
- Train : A csv of 784 features - Each feature being a pixel value for a 28*28 image. A target feature containing labels
- Test : A csv of 784 features - Each feature being a pixel value for a 28*28 image
- Sample Sumbission Csv - A sample submission file telling us how the submission file should look like

## Approach
Built a custom CNN model which had the following architecture

<img width="400" img height= "1200" alt="submission" src="https://github.com/siddh30/Digit_Recognizer-Kaggle_Competion/blob/main/model_plot.png"> 

## Tips thats really helped:

- Adding More Layers (Making the Network deeper to decrease training loss)
- Including Batch Norm, Max Pooling, Padding Layers
- Experimenting with different values of Dropout Regularization (to decrease Validation Loss and hence reduce overfitting)
- Experimenting with different bacth sizes (64 works best)
- Setting up Callbacks : -
  1. Learning Rate Scheduler to slow down learning as model reached Convergence
  2. Saving and Loading from the best model with focus on least validation loss
- Finally Ensembling results from various model runs to give a best aggregate results (Mode of prediction labels)

## Link to my Kaggle notebook 
https://www.kaggle.com/code/siddharthmandgi/digit-recognizer-above-0-99-score 


  
