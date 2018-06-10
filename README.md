# Few-Shot Charge Prediction with Discriminative Legal Attributes
Source code and datasets of COLING2018 paper: "Few-Shot Charge Prediction with Discriminative Legal Attributes"
## Dataset
The dataset takes space of 1.2GB, please download it [here](), and  put the folder "data" under this directory. It contains following files:

* words.vec: Pre-trained word embeddings, each line contains a word and its embedding. 
* attributes: The legal attributes for each charge.
* train: data for training.
* test: data for test.
* valid: data for validation.

## Run
Run the following command for training our model:

    cd code/
    python train.py

## Dependencies
* Tensorflow == 0.12
* Scipy == 0.18.1
* Numpy == 1.11.2

## Log
After start training,  a new folder "log" will be created.There are 4 directories in it:

* /evaluation_charge_log/: stores model's performance of charge prediction on test data during training.
* /evaluation_attr_log/: stores model's performance of attribute prediction on test data during training.
* /validation_charge_log/: stores model's performance of charge prediction on validation data during training.
* /validation_attr_log/: stores model's performance of attribute prediction on validation data during training.

## Cite
If you use the code, please cite this paper:
  
_Zikun Hu, Xiang Li, Cunchao Tu, Zhiyuan Liu, Maosong Sun. Few-Shot Charge Prediction with Discriminative Legal Attributes. The 27th Iinternational Conference on Computational Liguisitics (COLING 2018)._

For more related works on network representation learning, please refer to my [homepage](http://thunlp.org/~tcc/).