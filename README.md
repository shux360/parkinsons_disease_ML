<h1 align="left" id="title">Machine Learning Project : Parkinson's Disease Detection </h1>

<p id="description">We're excited to share our project with the world and invite you to join us in exploring the endless possibilities at the intersection of technology and finance which addresses a real-world need 💡</p>

  
  
<h2>Introduction</h2>

Parkinson's disease (PD) is the second most prevalent age-related neurological condition which causes a variety of physical and mental symptoms. It is challenging to diagnose Parkinson's disease (PD) because its symptoms are quite similar to those of other illnesses, like essential tremor and normal ageing. When a person reaches the age of 50, outward signs like trouble walking and speaking start to appear. Certain drugs relieve some of the symptoms of Parkinson's disease, despite the fact that there is a treatment available. By managing the complications brought on by the disease, patients are able to live their normal lives. Identifying the disease and stopping its progression are crucial at this stage.Parkinson's disease (PD) is a steadily deteriorating condition with symptoms that gradually arise over time, affects millions of people globally. About 10% of people exhibit symptoms of the disease before the age of 40, whereas prominent symptoms arise for those above 50 [1](https://www.healthdirect.gov.au/blog/parkinsons-disease-symptoms-in-your-30s-40s).

This project aims to build machine learning models to detect Parkinson's disease using biomedical voice measurements. In order to distinguish between healthy and PD patients based on voice signal characteristics, our project uses a two Machine Learning (ML) models, including Support Vector Machine (SVM), Random Forest Classifier(RF),195 voice recordings of examinations performed on 31 patients made up the dataset. In order to improve model performance, our models was trained using feature selection, hyperparameter tuning (GridSearchCV), feature scaling, and the Random Over-sampler.Evaluation techniques and metrics, including the Classification Report, F1-Score, Accuracy, Precision, Recall, and Confusion Matrix were used to evaluate the model performance.
  
  
<h2>Literature Survey</h2>

Parkinson's Disease is named after James Parkinson
a British physician in 1817 [3](https://pmc.ncbi.nlm.nih.gov/articles/PMC3234454/#:~:text=Parkinson's%20disease%20was%20first%20medically,earlier%20descriptions%20(Parkinson%201817).). It has been proven that machine learning techniques are effective in detecting Parkinson's disease early on. These algorithms have been used for many years to diagnose diseases. For example, Lafunte and his colleagues used ANN in 1997 to separate individuals with lower limb arthritis from those in good health with 80% accuracy [4](https://www.sciencedirect.com/science/article/abs/pii/S026800339700082X). Using a collection of biological voice signals from both healthy and Parkinson samples, A. Sharma et al. (2014) applied pattern recognition, neural networks, and support vector machines to diagnose Parkinson's disease (PD) with an accuracy of 85.294% [5](https://pmc.ncbi.nlm.nih.gov/articles/PMC8134676/).
Another study was conducted in 2020, and the results showed that PD patients could be differentiated from healthy people at an early stage of the disease with accuracy rates of 93.5%, 96%, and 95.2% using features such as RMS, chroma STFT, spectral centroid, etc [6](https://www.revistaclinicapsicologica.com/archivesarticle.php?id=494).

<h2>Dataset Description</h2>

This dataset is composed of a range of biomedical voice measurements from 31 people, 23 with Parkinson's disease (PD). Each column in the table is a particular voice measure, and each row corresponds to one of 195 voice recordings from these individuals ("name" column). The main aim of the data is to discriminate healthy people from those with PD, according to the "status" column which is set to 0 for healthy and 1 for PD.

**Matrix column entries (attributes):**
*   name - ASCII subject name and recording number
*   MDVP:Fo(Hz) - Average vocal fundamental frequency
*   MDVP:Fhi(Hz) - Maximum vocal fundamental frequency
*   MDVP:Flo(Hz) - Minimum vocal fundamental frequency
*   MDVP:Jitter(%),MDVP:Jitter(Abs),MDVP:RAP,MDVP:PPQ,Jitter:DDP - Several
measures of variation in fundamental frequency
*   MDVP:Shimmer,MDVP:Shimmer(dB),Shimmer:APQ3,Shimmer:APQ5,MDVP:APQ,Shimmer:DDA - Several measures of variation in amplitude
*   NHR,HNR - Two measures of ratio of noise to tonal components in the voice
*   status - Health status of the subject (one) - Parkinson's, (zero) - healthy
*   RPDE,D2 - Two nonlinear dynamical complexity measures
*   DFA - Signal fractal scaling exponent
*   spread1,spread2,PPE - Three nonlinear measures of fundamental frequency variation'

**Models**
*   SVM - Support Vector Machine
*   KNN - K Nearest Neighbors Classification

**Accuracies**
*   SVM: Training Accuracy: 0.94, Testing Accuracy: 0.90
*   KNN: Training Accuracy: 0.95, Testing Accuracy: 0.92









