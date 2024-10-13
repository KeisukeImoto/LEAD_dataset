# LEAD dataset

## What is LEAD dataset [1]?
The Lead dataset contains strong labels for sound events, in which each clip has 20 different annotations.
The LEAD dataset allows us to investigate how strong labels vary from annotator to annotator and consider SED models that are robust to the variation of strong labels.
The sound clips for the LEAD dataset are selected from all of TUT Sound Events 2016/2017, parts of TUT Acoustic Scenes 2016, and URBAN-SED. 

## Dataset discription

The dataset consists of strong labels assigned to sounds in TUT Sound Events 2016/2017 [2][3], a part of TUT Acoustic Scenes 2016 [2], and a part of URBAN-SED [4]. 
For TUT Sound Events 2016/2017, we used all sound clips, which includes 2.9 h of sounds (47 files), whereas for TUT Acoustic Scenes 2016, we used a subset that includes all 15 acoustic scenes, which contains 2.6 h of sounds (314 files). For URBAN-SED, we used 0.17 h of sounds (60 files).
For each sound clip, 20 annotators assigned sound event labels and gave their onset/offset.
For TUT Sound Events 2016/2017 and TUT Acoustic Scenes 2016, we provided 20 candidate event labels for each acoustic scene, and the annotators selected the most suitable event labels from the candidates and then gave onsets/offsets. 
The annotators also assigned two confidence scores: one is the confidence score for selecting the type of sound event and the other is for providing the onset and offset of the sound event.
These confidence scores are attributed to each sound event instance. 
We set the confidence score on a five-point scale ranging from 1 (very unconfident) to 5 (very confident).
The annotators were asked to listen to an entire sound clip at least once during the annotation and to refer to a waveform plot and/or spectrogram if necessary.
The annotators were instructed to consider sound events occurring at intervals of more than 1 s as different sound events.

The annotations of the LEAD dataset are organized in the same tsv format as those of TUT Sound Events 2016/2017 and TUT Acoustic Scenes 2016, except for the confidence scores (CSs) to the sound event class and the onset/offset of each sound event instance, as follows.

```
event_start_time	event_end_time	event_label	 CS for selecting sound events  CS for providing onset/offset
0.619375      12.304331      car                4       3
1.671731      224.798167     bird singing       5       4
3.926606      5.889908       (object) impact    3       3
7.616967      44.334651      people walking     4       4
```

Note that sound files of the TUT Sound Events 2016/2017, TUT Acoustic Scenes 2016, and URBAN-SED are not included in this dataset. Please download them from the DCASE Challenge Web page (or directly Zenodo).


## Download link for audio data of TUT Sound Events 2016/2017, TUT Acoustic Scenes 2016, and URBAN-SED

TUT Sound Events 2016, Development dataset: https://zenodo.org/records/45759  
TUT Sound Events 2016, Evaluation dataset: https://zenodo.org/records/996424  
TUT Sound Events 2017, Development dataset: https://zenodo.org/records/400516  
TUT Sound Events 2017, Evaluation dataset: https://zenodo.org/records/1040179  
TUT Acoustic Scenes 2016, Development dataset: https://zenodo.org/records/45739  
TUT Acoustic Scenes 2016, Evaluation dataset: https://zenodo.org/records/165995  
URBAN-SED: https://urbansed.weebly.com/

##

[2]  A. Mesaros, T. Heittola, and T. Virtanen, “TUT Database for Acoustic Scene Classification and Sound Event Detection," Proc. European Signal Processing Conference (EUSIPCO), pp. 1128-1132.  
[3]  A. Mesaros, T. Heittola, A. Diment, B. Elizalde, A. Shah, B. Raj, and T. Virtanen, “DCASE 2017 challenge setup: Tasks, datasets and baseline system,” Proc. Workshop on Detection and Classification of Acoustic Scenes and Events (DCASE) Workshop, pp. 85-92, 2017.
