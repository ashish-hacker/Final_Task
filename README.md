# Project Report :

Spectrum Internship Drive is one month long Internship . Where internees were given Resources to learn Machine Learning and Projects in a regular Interval. 
### Task 0:
First a pretask was given to warmup our brains about the tools I was about to use. The whole project was upon the character Billy.The task I did is eased the work of Billy. In the pretask I Plotted the graph scores vs days using matplotlib and found out the mean, median ,minimum and maximum scores using Numpy.

### Task 1:


### Final Task:
In this Task I had two sub tasks:
        1.Importing Data and getting the dummy variable for all the non-numeric features. And then Splitting it into Training Data and Testing Data.
        2.Create a model , Fit the model using the training Data and predict the outputs by feeding the Test Data to the model we have trained before.Then to improve accuracy ,I had to eliminate the features which are not affecting the prediction , By Backward Elimination. Then noting the accuracy.

For Importing the Data and getting dummy variable , I have used Panads library of python.And for Model I have used LinearRegression which comes from sklearn's linear_model library. For Backward Elimination I have used statsmodel.api.For cross-validation I have used ShuffleSplit. And with pipeline from sklearn I have used svm's linearSVR model to fit my cross-validated Data.
I Noted that unscaled data with LinearRegression model at first had an accuracy of 97.09% .Then after Backward Elimination I got an accuracy of 97.56%.Then I scaled the Data.We are using Scaler here for scaling our data. What it does is Standardize the dataset & Center to the mean and component wise scale to unit variance.But we got almost same accuracy.Its because our Data is small I guess.
        
        
