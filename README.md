# Project Report :

**Spectrum Internship Drive** is one month long Internship . Where internees were given Resources to learn *Machine Learning* and Projects in a regular Interval. 
### Task 0:
First a pretask was given to warmup our brains about the tools I was about to use. The whole project was upon the character Billy.The task I did is eased the work of Billy. In the pretask I Plotted the graph scores vs days using matplotlib and found out the mean, median ,minimum and maximum scores using Numpy.

### Task 1:


### Final Task:
In this Task I had two sub tasks:
        1.Importing Data and getting the dummy variable for all the non-numeric features. And then Splitting it into Training Data and Testing Data.
        2.Create a model , Fit the model using the training Data and predict the outputs by feeding the Test Data to the model we have trained before.Then to improve accuracy ,I had to eliminate the features which are not affecting the prediction , By Backward Elimination. Then noting the accuracy.

For Importing the Data and getting dummy variable , I have used *Panads* library of python.And for Model I have used *LinearRegression* which comes from *sklearn's linear_model* library. For Backward Elimination I have used *statsmodel.api*.For cross-validation I have used *ShuffleSplit*. And with pipeline from sklearn I have used svm's *linearSVR* model to fit my cross-validated Data.
I Noted that unscaled data with LinearRegression model at first had an accuracy of **97.09%** .Then after Backward Elimination I got an accuracy of **97.56%**.Then I scaled the Data.We are using *Scaler* here for scaling our data. What it does is Standardize the dataset & Center to the mean and component wise scale to unit variance.But we got almost same accuracy.Its because our Data is small I guess.
Learning the parameters of a prediction function and testing it on the same data is a methodological mistake: a model that would just repeat the labels of the samples that it has just seen would have a perfect score but would fail to predict anything useful on yet-unseen data. This situation is called overfitting. To avoid it, it is common practice when performing a (supervised) machine learning experiment to hold out part of the available data as a test set X_test, y_test.Which can be done by **Cross-Validation**.I made a pipeline then added *StandardScaler* and the model *LinearSVR* to it. And then I fitted the model with the scaled training Data.Then I noted the accuracy, It was over **98%**.

## Some Insights From The Data:

* Obviously, G1,G2 are more valuable features in the Data for predicting The Final Grade. Because, The grades add up to give The Final Grade , thats why The final Grade is directly depend upon the grades G1, G2, G3.
* Then I plotted between various features and the Final grade. It was clearly visible that increasing age decreases the Final Grade of the students. And the Age group of 20 topped on average.
* The students who are not indulged in romantic affairs scored better on average.
* If Mother of the student is working in Health, public services or teacher proffession scored better. Children of Health department Mothers scored better than others.
* If Father is a teacher the student child scored better .
* Students Who are healthy scored higher .
* Students who bunked more classes , got lesser grades.
* Students who study more hours weekly got better grades.
* Students who didn't failed much in previous classes got better grades.
* From the Data it Looks like Gabriel Pereira School Students Score Better than Mousinho da Silveira School Students.
* If The Guardian is Other Than The Parents, Students Score Lesser.
* Students Having Extra Paid Classes within the Course Subjects Score Better.
* Students who don't go out often score higher.
* Students who had more freetime got better grades.
* Students Who Have Ambitions For Higher Education, Score Higher.
* Boys score better than girls.
* Urban Area Students Are Scoring Higher Than Students In Rural Area.
        
        
