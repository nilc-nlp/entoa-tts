# FastSpeech2
Repo: https://github.com/sidleal/FastSpeech2

# CMLTTS Checkpoint
The portuguese part of CMLTTS, with 30 speakers
````
Step 720000, Total Loss: 1.3474, Mel Loss: 0.5014, Mel PostNet Loss: 0.5004, Pitch Loss: 0.1153, Energy Loss: 0.1592, Duration Loss: 0.0710
````
Using:
````
python synthesize.py --text "porque a televisão é horroroso quando eles estão fazendo programa."  \
 --speaker_id 25 --restore_step 720000 --mode single -p config/cmltts/preprocess.yaml \
 -m config/cmltts/model.yaml -t config/cmltts/train.yaml
````

# CMLTTS_333 Checkpoint
CMLTTS 30 speakers + prosodic D2_333_TB-L1 speaker
````
Step 720000, Total Loss: 1.7945, Mel Loss: 0.5951, Mel PostNet Loss: 0.5939, Pitch Loss: 0.1929, Energy Loss: 0.3127, Duration Loss: 0.0999
````
Using:
````
python synthesize.py --text "porque a televisão é horroroso quando eles estão fazendo programa."  \
 --speaker_id 7 --restore_step 720000 --mode single -p config/cmltts_333/preprocess.yaml \
 -m config/cmltts_333/model.yaml -t config/cmltts_333/train.yaml
````

# CMLTTS_ENTOA_PROS Checkpoint
CMLTTS 30 speakers + 39 prosodic speakers (entoa-tts-prosodic excluding DID_234_L1) 
````
Step 720000, Total Loss: 2.2516, Mel Loss: 0.5903, Mel PostNet Loss: 0.5890, Pitch Loss: 0.3196, Energy Loss: 0.6478, Duration Loss: 0.1049
````
Using:
````
python synthesize.py --text "porque a televisão é horroroso quando eles estão fazendo programa."  \
 --speaker_id 54 --restore_step 720000 --mode single -p config/cmltts_entoa_pros/preprocess.yaml \
 -m config/cmltts_entoa_pros/model.yaml -t config/cmltts_entoa_pros/train.yaml
cmltts_entoa_pros``
