# MpbPPI
A multi-task pre-training-based equivariant approach for the prediction of the effect of amino acid mutations on protein-protein interactions

How to use it:

Basic Environment:
* __Python 3.9.13__
* __Pytorch 1.12.1__
* __CUDA tool kit 11.3.1__
* __Pytorch Geometric (PyG) for PyTorch 1.12.* and CUDA 11.3__


Step1. __Download our pre-processed jsonl file from https://drive.google.com/file/d/1Y_3xn5qrnYG79CiQAJKPrw2coL3DSax3/view?usp=sharing, and put it into ./data/ folder as the source data file.__

Step3. __Follow the illustration in _4_run_MpbPPI_ddg_prediction.py file, to read the above jsonl file_



the model input generated by above two .ipynb files (e.g., files in provided 'fold1') and  run&evaluate different variants described in the manuscript (after training the model, these .py files will automatically evaluate the model performance on the test set):__
