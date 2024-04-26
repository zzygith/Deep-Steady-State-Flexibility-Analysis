# PyTorch implementation of Deep-Steady-State-Flexibility-Analysis

## Installation
This code is written in `Python 3.7` and requires the packages listed in `requirements.txt`.

Clone the repository to your local machine and run the code:
```
git clone https://github.com/zzygith/Deep-Steady-State-Flexibility-Analysis.git
cd <path-to-Deep-Steady-State-Flexibility-Analysis-directory>
pip install -r requirements.txt
mkdir log/ro_test
cd src
# select one case
python main.py mine_heater_1d mine_net1D ../log/ro_test ../data/mine_heater_1d.txt --n_epochs 300 --pretrain False --lr 0.001
# or
python main.py mine_reactorCooler_2d mine_netRC2D ../log/ro_test ../data/mine_reactorCooler_2d.txt --n_epochs 200 --pretrain False --lr 0.001
# or
python main.py mine_reactorCooler_5d mine_netRC5D ../log/ro_test ../data/mine_reactorCooler_5d.txt --n_epochs 200 --pretrain False --lr 0.0001;
```
## License
MIT