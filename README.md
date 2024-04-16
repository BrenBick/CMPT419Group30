# CMPT419Group30
Group 30 Project Files for CMPT 419


## 1. Installation

The following libraries are required to run the code.

```bash
git clone $THISREPO
cd $THISREPO
pip3 install opencv-python
pip3 install ultralytics
pip3 install tensorflow
pip3 install moviepy
pip3 install librosa
```

### What to find where


```bash
repository
├── src                     ## source code of the package itself
	├── data                ## Directory for the video clip training dataset
	    ├── Surprised     
	    ├── Frustrated
	    ├── Embarrassed
	    ├── Confused
	    ├── frames		## This is where the extracted images will be stored
	├── load_data.ipynb		## This notebook extracts the image frames from the videos in the data folder
	├── label.csv			## This contains the path and labels for every video clip in the dataset
	├── image-model			   ## Directory for training the image sub-model
	  ├── dataset
	    ├── train           ## Training data directory for the image frames
	        ├── Surprised     
	        ├── Frustrated
	        ├── Embarrassed
	        ├── Confused
	    ├── test           ## Validation data directory for the image frames
	        ├── Surprised     
	        ├── Frustrated
	        ├── Embarrassed
	        ├── Confused
	  ├── runs             ## Statistics from training the image model
	├── make-prediction    ## Main directory for making a prediction THIS IS WHERE YOU CAN TEST
	  ├── emoji_output.ipynb ## Notebook for making aprediction on a video
	  ├── video.mp4         ## The video you want to predict for
├── README.md       			## You are here
```
