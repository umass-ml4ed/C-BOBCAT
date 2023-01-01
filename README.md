# C-BOBCAT: Constrained Version of Bilevel Optimization-Based Computerized Adaptive Testing
### Environment Setup
This repository uses the following Pytorch version in Python3.
``` bash
torch==1.12.1
```
### Data
You can download the preprocessed datasets from [Google Drive](https://drive.google.com/file/d/18jMoNc12cfngyD796YITRiEp1KIq4oVu/view?usp=sharing) to `/data/` folder. Preprocessing scirpts can be found in `utils/` folder.
### Training
``` bash
python train.py
    --dataset {mapt-math, mapt-read}
    --model {binn-biased, biirt-biased}
    --n_query {2, 4, 8}
    --lamda {0.003, 0.001, 0.03, 0.01}
    --cuda
    --gumbel
    
```
