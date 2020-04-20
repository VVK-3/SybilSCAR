The code is used to compute commonly used metrics: 

Area Under the ROC Curve (AUC);
False Positive Rate (FPR); 
False Negative Rate (FNR); 
True Positive Rate (TPR); 
True Negative Rate (TNR); 
Accuracy (ACC) = (TP+TN) / (TP+TN+FP+RN);

AUC is used to evaluate ranking, while the remaining metrics are used to evaluate classification.
we define benign as positive and Sybil as negative. Therefore, FPR means the fraction of Sybils that are predicted as benign, while FNR is the fraction of benign nodes that are predicted as Sybils.  

Input Files
----------------
1. test file
2. post file

Expected output
----------------
the output values lies between 0 and 1
AUC XXX
ACC XXX
FPR XXX
TPR XXX
FNR XXX
TNR XXX

How to do it
-----------------
Compile: g++ metric.cpp -O3 -o metric

Execute: ./metric -testfile TESTFILE -postfile POSTFILE

The above lines are used to verify the individual file so for the project please refer Final_readme.
