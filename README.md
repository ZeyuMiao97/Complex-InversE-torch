# Complex-InversE-torch
Run ED-SimplE with Pytorch
# Summary
This software can be used to run Complex-InversE on datasets FB15k-237 and WN18RR with Pytorch.
# Installation
1. Install PyTorch using Anaconda.
2. Install the requirements `pip install -r requirements.txt`
3. Download the default English model used by spaCy, which is installed in the previous step `python -m spacy download en`
4. Run the preprocessing script for WN18RR, FB15k-237: `preprocess.sh`
5. You can now run the model
# Running a model
Parameters need to be specified by white-space tuples for example:  
  
`python main.py --model Complex-InversE --data FB15k-237`  
  
will run a Complex-InversE model on FB15k-237.  

To run a model, you first need to preprocess the data once. This can be done by specifying the `--preprocess` parameter:  

`python main.py --data DATASET_NAME --preprocess`   
  
After the dataset is preprocessed it will be saved to disk and this parameter can be omitted.  

The following parameters can be used for the `--model` parameter:  
  
`Complex-InversE`  
`distmult`  
`complex`  
  
The following datasets can be used for the `--data` parameter:  
  
`FB15k-237`  
`WN18RR`  
