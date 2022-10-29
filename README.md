<div align="center">
  
# Binary Sequence Classification using BERT

</div align="center">

---

> This is the official repository of my submission to the [StumbleUpon Evergreen Classification Challenge](https://www.kaggle.com/competitions/stumbleupon/overview).

---

This is a Binary sequence classification problem where we need to differentiate
a paragraph upon its ability to stay relevant through times i.e. evergreen or ephemeral.

The main approach I used to solve the problem is using BERT (Bidirectional Encoder Representations from Transformers)
for sequence classification which is a pretrained word embedding transformer in pytorch.

## Dataset:
1. The dataset can be downloaded from this [link](https://www.kaggle.com/competitions/stumbleupon/data).

## Training
1. Run the stumbleupon.ipynb file.

## Evaluation
1. For evaluation, the model is evaluated on the validation dataset and the corresponding 
classification report is generated with precision and recall for each classes.
2. Running all the cell blocks from the stumbleupon.ipynb file which generate the results.

## Results

Class based classfication report (on the validation dataset):

|Class        | Precision | Recall | F1 score | Supporting Samples|
--------------|-----------|--------|----------|-------------------|
|Non Evergreen|0.77       |0.83    |0.80      |540                |
|Evergreen    |0.83       |0.77    |0.80      |570                |

## Contact
For any queries, feel free to contact at vignesh.nitt10@gmail.com.
