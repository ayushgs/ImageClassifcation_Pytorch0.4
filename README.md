# ImageClassifcation_Pytorch0.4

This repository contains necessary codes to establish a neural image classification pipeline by a model architecture of one's choice. The codes can be used a reference by beginners to build their own model. 


### main.ipynb

To aid in the learning process for beginners, all the codes have been placed in a single Ipython notebook for easy lookup.  


### data_utils.py

Some utility files used by the main code, mainly related to the data loading and processing pipelines. Other helper function have been defined in the main file itself.

### get_datasets.sh
A bash scripts to download the CIFAR 10 dataset. Add the following command to the terminal to download the entire data and move it to a directory of your choice from which you access this data in the main Ipython notebook.
```
cd <the containing directory>
./get_datasets.sh
#run chmod a+x *.* if the script does not run to make it executable
```
### To add to GPU
Though I did not have a GPU resource while building this code, training the model on a NVIDIA GPU can be achieved easily in pytorch.  Append this code in the starting for the same.

```
use_cuda = False
device   = torch.device('cpu')
if torch.cuda.is_available():
use_cuda = True
device   = torch.device('cuda')
```

### P.S.:
The model wasn't trained for long enough, hence the training graphs in the Ipython notebook are nothing more than for represeting code structure. Also, since the models were'nt trained for long enough, I haven't added any pre-trained weights or checkpoints. 

Do take care of amending the correct file paths for your personal use. 

## Acknowledgments
Hat tip to anyone who's codelines were used in any part of the code. Your code was an inspiration! :)
