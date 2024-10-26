#Team AI Or Not

##Members

- Jacques Castonguay
- Mihal Zavalani
- Safa Khatoon

##Sources
CNN design:
https://learn.microsoft.com/en-us/windows/ai/windows-ml/tutorials/pytorch-train-model
Dataset:
https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images

##Steps: 0. Optional - run in a virtual environment (Windows)

- open terminal in this project space/folder
- create a virtual environment: `python -m venv myenv`
- enter environment: `myenv\Scripts\activate` or if using powershell: `myenv\Scripts\Activate.ps1`
- when you want to leave the virtual env: `deactivate`

1. Download our dataset listed above. Unzip it. Move it to this folder and rename to archive_0 (or you can rename the root dir when training our model)

2. Download requirements: `pip install -r requirements.txt`. May need to use pip3 instead

3. (Can skip to real dataset if desired) Run PyTorchTraining.py with `python ./PyTorchTraining.py`. You may need to use python3 instead.

- This is the test model that is made in the tutorial. Try different Epochs. Tutorial used 2. 10 gave best results but took a while to train. The first time this is ran the CiFar model will be downloaded, if re-ran it will use the saved images previously downloaded. Model weights are saved as myFirstModel.pth

4. Real dataset. Run aiOrNot.py with `python ./aiOrNot.py`. Model weights are saved as aiOrNot.pth
