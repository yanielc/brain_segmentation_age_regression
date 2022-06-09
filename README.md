# Two deep learning approaches to age prediction using brain MRIs.


We study two different methods to predict the age of patients based on the brain MRIs. 

In the first case we assume there is a brain segmentation model which can differentiate grey matter (GM), white matter (WM), and cerebrospinal fluid (CSF). We first train the model (a simple U-net) and then use the predicted volumes for each tissue type as regressors for the age of the patient.

In the second case, we use the images themselves as input to a network which regresses the age. This model outperforms the 2-step case above which attests to the flexibility and power of neural networks as end-to-end models. The case above though shows that given a segmentation model we do not need to train a new model necessarily, but instead build on top of it. 
