# MpbPPI
### A multi-task pre-training-based equivariant approach for the prediction of the effect of amino acid mutations on protein-protein interactions

__How to use it:__

__Basic Environment (Windows or Linux):__
* Python 3.9.13
* Pytorch 1.12.1
* CUDA tool kit 11.3.1
* Pytorch Geometric (PyG) for PyTorch 1.12.* and CUDA 11.3


Step1. __Download our pre-processed jsonl file (generated based on the mutant-type (MT) PPI complex source FoldX) from https://drive.google.com/file/d/1Y_3xn5qrnYG79CiQAJKPrw2coL3DSax3/view?usp=sharing, and put it into ./data/ folder as the downstream source data file.__

Step2. __Follow the illustration in \_4_run_MpbPPI_ddg_prediction.py, to read the above jsonl file and run&evaluate MpbPPI for downstream ddG predictions in two different data splitting ways.__

__A running example (including training and evaluation to create the similar results reported in the manuscript):__

__After the environment configuration, usually several hours are needed to finish running the demo code.__

python \_4_run_MpbPPI_ddg_prediction.py --data_split_mode 'CV10_random' (mutation-level tenfold cross-validation)

python \_4_run_MpbPPI_ddg_prediction.py --data_split_mode 'complex' (wide-type PPI complex type-based cross-validation)

__The scripts for the full pre-processing pipeline as well as our collected pre-training data and corresponding pre-training script will be released upon acceptance.__

### MIT License

Copyright (c) [2023] [Yang Yue]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.



