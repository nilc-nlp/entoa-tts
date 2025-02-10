# FastSpeech2
Repo: https://github.com/sidleal/FastSpeech2

# CMLTTS Checkpoint
````
Step 720000, Total Loss: 1.3474, Mel Loss: 0.5014, Mel PostNet Loss: 0.5004, Pitch Loss: 0.1153, Energy Loss: 0.1592, Duration Loss: 0.0710
````
Using:
````
python synthesize.py --text "porque a televisão é horroroso quando eles estão fazendo programa."  \
 --speaker_id 25 --restore_step 720000 --mode single -p config/cmltts/preprocess.yaml \
 -m config/cmltts/model.yaml -t config/cmltts/train.yaml
````
