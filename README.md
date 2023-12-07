# DAMS
A Multimodal Emotion Recognition Method Based on Dual-Layer Asymmetric Multi-Head Attention and Spatial Mapping
## Requirements
   tensorflow-gpu==1.14.0 <br>
   torch == 1.2.0 <br>
   transformers==2.10.0 <br>
   numpy==1.15.4 <br>
   sklearn <br>
   python 3.6.13 <br>   cudatoolkit==9.2<br>

## Usage


* download processed features from [Google Drive](https://drive.google.com/drive/folders/1Q-NujC2-Egyq2GUO2Ipy9z59MSeY1mmb?usp=drive_link) or [Baidu Disk]( https://pan.baidu.com/s/1BJZkg8nNElFg9KSXdrLlyw?pwd=2qiu) 

* or process file by [OpenSimle2.0](https://github.com/audeering/opensmile), Bert, and [Librosa](https://github.com/librosa/librosa). Refer to utils folder.

* download saved_model from [Google Drive](https://drive.google.com/drive/folders/1r9zzLFMl1tsgo7lKYpcYIsfrGuUPpXvk?usp=drive_link) or [Baidu Disk]( https://pan.baidu.com/s/1BJZkg8nNElFg9KSXdrLlyw?pwd=2qiu) 

* generate train.pkl and test.pkl
```python 
python Dataset.py
```
* train (can modify settings in Settings.py) <br>
```python 
python train.py  
```
* As for the IEMOCAP dataset, replacing the Datset.py, network.py and train.py in the iemocap folder.

* test <br>
```python 
python train.py --train=False
```
