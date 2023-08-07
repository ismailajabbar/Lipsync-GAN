# Lipsync - GAN

## Readme
Original readme file has been renamed to "Original_README.md"

## Install Libraries
Use command below to install necessary requirements (tested locally).
```
pip install requirements.txt
```

Original requirements.txt file have been renamed to "Original_requirements.txt"

## Prepare Weights
- Face detection [pre-trained model](https://www.adrianbulat.com/downloads/python-fan/s3fd-619a316812.pth) should be downloaded, moved, and renamed to `face_detection/detection/sfd/s3fd.pth`. Alternative [link](https://iiitaphyd-my.sharepoint.com/:u:/g/personal/prajwal_k_research_iiit_ac_in/EZsy6qWuivtDnANIG73iHjIBjMSoojcIV0NULXV-yiuiIg?e=qTasa8) if the above does not work.

- | Wav2Lip + GAN  | Slightly inferior lip-sync, but better visual quality | [Link](https://iiitaphyd-my.sharepoint.com/:u:/g/personal/radrabha_m_research_iiit_ac_in/EdjI7bZlgApMqsVoEUUXpLsBxqXbn5z8VTmoxp55YNDcIA?e=n9ljGW) | Put the file inside the "checkpoints" folder.



## Predict
Testing file are placed inside the "test_input" folder.
```
python inference.py --checkpoint_path checkpoints/wav2lip_gan.pth --face "test_input/Kohli_input_video.mp4" --audio "Lipsync/Kohli-subhramanyam.mp3" --pads 0 20 0 0    
python inference.py --checkpoint_path checkpoints/wav2lip_gan.pth --face "test_input/Kohli_input_video.mp4" --audio "Lipsync/Kohli-subhramanyam.mp3" --pads 0 20 0 0
python inference.py --checkpoint_path checkpoints/wav2lip_gan.pth --face "test_input/Kohli_input_video.mp4" --audio "Lipsync/Kohli-subhramanyam.mp3" --pads 0 20 0 0
```

## Results
See "results" folder for previous testing results.
