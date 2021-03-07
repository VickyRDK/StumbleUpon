# StumbleUpon

* The StumbleUpon Challenge is a binary sequence classification problem where we need to differentiate
a paragraph upon its ability to stay relevant through times i.e. evergreen or ephemeral.

* The main approach I used to solve the problem is using BERT (Bidirectional Encoder Representations from Transformers)
for sequence classification which is a pretrained word embedding transformer in pytorch.

### Approach of Solving:

* Dataset is split into training and validation sets.

* BERT can load only 512 words at a time. So we need to upload the important details from the
boilerplate text. SO we filter out the last 512 words from the body as they conclude the statement and so has more
weight to it.

* Tokenizer is initialized from the BERT pretrained model and then we retrieve word embeddings
from it by encoding the validation and train data.

* Some normal helper function are coded to ease the process of training.

* After training, the model is evaluated on the validation dataset and the corresponding 
classification report is generated with precision and recall for each classes.

(This was coded in google colab as my gpu was unable to load the dataset)
