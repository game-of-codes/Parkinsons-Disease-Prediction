# Parkinsons-Disease-Prediction

Parkinson’s disease is a neuro-degenerative disorder which affects quality of life of
an estimated 10 million people worldwide3
. A tell-tale marker of this disease is a
decrease in the dopamine levels in the brain which could be attributed to the
degeneration of dopaminergic neurons. The onset of the disease may be suggested
by tremor, rigidity, slowness of movement and postural instability14. Such symptoms
may not present itself in the same format in all the cases but rather vary in
combinations and severity but generally is chronic and degenerative. What interests
us here is that among all diagnosed cases of PD, 90% of the cases show some sort
of vocal impairment which consists of deterioration of normal production of vocal
sounds, which is medically termed as Dysphonia

As PD patients
show unique and characteristic vocal features, their voice recordings would prove to
be an invaluable procedure for diagnosis as it is also non-invasive. Hence tests using
speech prove to be a good tool to audit PD. This opens up an entirely new door of
opportunities for Machine Learning algorithms to work on in-house voice recording
datasets of PD patients and then go on to efficiently predict or diagnose PD20
. Voice
features from the audio clips can be extracted by passing the recordings through
signal processing algorithms and a these features can be used to build a classification
and regression model to predict a rating on the Unified Parkinson’s Disease Rating
Scale (UPDRS)15. UPDRS, which indicates presence and progression of PD, has
been as the most commonly used scale for measuring and assessing PD.

The dataset is taken from the UCI ML repository. Exploratory data analysis is done
long with visualizations of attributes to understand how the data characteristics of
the data

The dataset used in this study is collection of features from voice recordings taken
from 42 candidates who have been diagnosed with early-stage Parkinson's disease
recruited to a six-month trial of a telemonitoring device for remote symptom
progression monitoring. These recordings were captured by the device at the homes 
of the patients. Each row in the dataset corresponds to one of 5,875 voice recording
from the aforementioned individuals.
The objective of this study is to predict the motor and total UPDRS scores
('motor_UPDRS' and 'total_UPDRS') from the 16 vocal attributes which will give
an idea about the progression of PD.
The attributes in the dataset:
(i) Subject number:
Unique Id of each individual
(ii) Subject Age:
Age of the patient
(iii) Subject gender:
‘0’ indicates male, ‘1’ indicates female
(iv) Test time:
Time since the individual has been recruited into the trial.
(v) UPDRS:
This is a clinician’s scale for recording symptoms related to Parkinson’s
disease. The UPDRS metric is a scale with 44 sections, and each of those
sections addresses a symptom at one different part of the body. A summation
of these 44 section will yield a value called UPDRS score which ranges
between 0 (perfectly healthy) to 176(total disability)
(vi) Motor UPDRS:
Motor UPDRS score given by the clinician, linearly interpolated - this forms
sections 18-44 from the UPDRS sections
(vii) Total_UPDRS:
total UPDRS score given by clinician, linearly interpolated - this includes all
44 sections.
(viii) 16 other biomedical voice measures such as :
Jitter Percentage, Jitter (Absolute), Jitter (RAP), Jitter (PPQ5), Jitter (DDP),
Shimmer, Shimmer(dB), Shimmer:APQ3, Shimmer:APQ5,
Shimmer:APQ11, Shimmer: DDA, NHR, HNR, RPDE, DFA, PPE


Prediction:
The objective of this study is to accurately predict the motor and total UPDRS scores
('motor_UPDRS' and 'total_UPDRS') from the 16 voice measures using various
machine learning methods and compare the results. For the same purpose we will be
making use of SVM, Random Forest, Linear Regression and Multi-Variate Linear
regression. We’ve used Root Mean Squared Error (RMSE). RMSE is defined as the 
square root of the average of the square of the total error. It’s one of the most
common uses measure of accuracy for prediction problems.
