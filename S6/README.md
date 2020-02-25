## Team: 
#### Deep&Dark
## Team Member: 
#### Prachi, Harsha, Abhinav, Chandan

##Note:

1. Graph of all no_reg, L1, L2, L1+L2 regularization loss and accuracy for train and test in ipython notebook(image in the folder)
2. Misclassified images of L1 and L2 are in the end of the notebook(image also in the folder)

## Analysis:

1. On this dataset, l1 regularization and L1+L2 is not working as expected. L1 seems to supersede L2 regularization. Model stops learning and accuracy does not improve. why?
2. l2 regularization and without regularization model are better models. 


Regularization	| Best Train Accuracy 	| Test Accuracy  
----- |-------|---
None|	99.19%|	99.64%
L1|	98.23%|	98.83%
L2|	99.17%|	99.58%
Both|	98.19%|	98.92%
