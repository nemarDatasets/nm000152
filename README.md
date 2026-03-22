# Upper-limb elbow-centered motor imagery dataset (10 classes)

Upper-limb elbow-centered motor imagery dataset (10 classes).

## Dataset Overview

- **Code**: Zhang2017
- **Paradigm**: imagery
- **DOI**: 10.1371/journal.pone.0188293
- **Subjects**: 12
- **Sessions per subject**: 1
- **Events**: rest=1, elbow_flexion=2, drawer=3, soup=4, weight_lifting=5, door=6, plate_cleaning=7, combing=8, pizza_cutting=9, pick_and_place=10
- **Trial interval**: [0, 4] s
- **Runs per session**: 15
- **File format**: BCI2000

## Acquisition

- **Sampling rate**: 1000.0 Hz
- **Number of channels**: 17
- **Channel types**: eeg=17
- **Hardware**: EGI Geodesic Net Amps 400 series (N400)
- **Software**: BCI2000 (Stimulus Presentation mode)
- **Reference**: Cz
- **Ground**: COM
- **Sensor type**: Ag/AgCl sponge
- **Line frequency**: 60.0 Hz
- **Online filters**: {'bandpass': [0.1, 40]}

## Participants

- **Number of subjects**: 12
- **Health status**: healthy
- **Age**: min=20, max=33
- **Gender distribution**: male=10, female=2
- **Handedness**: {'right': 11, 'left': 1}
- **BCI experience**: naive
- **Species**: human

## Experimental Protocol

- **Paradigm**: imagery
- **Number of classes**: 10
- **Class labels**: rest, elbow_flexion, drawer, soup, weight_lifting, door, plate_cleaning, combing, pizza_cutting, pick_and_place
- **Trial duration**: 5.0 s
- **Study design**: Upper-limb elbow-centered motor imagery with 9 goal-directed tasks plus rest. Each trial: 4-6 s cue (randomized) then 4-6 s rest (randomized).
- **Feedback type**: none
- **Stimulus type**: picture cues
- **Stimulus modalities**: visual
- **Primary modality**: visual
- **Synchronicity**: synchronous
- **Mode**: offline
- **Instructions**: Participants were asked to repetitively perform the kinesthetic motor imagery task displayed on the screen without actually moving.

## HED Event Annotations

Schema: HED 8.4.0 | Browse: https://www.hedtags.org/hed-schema-browser

```
  rest
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Rest

  elbow_flexion
    ├─ Sensory-event
    └─ Label/elbow_flexion

  drawer
    ├─ Sensory-event
    └─ Label/drawer

  soup
    ├─ Sensory-event
    └─ Label/soup

  weight_lifting
    ├─ Sensory-event
    └─ Label/weight_lifting

  door
    ├─ Sensory-event
    └─ Label/door

  plate_cleaning
    ├─ Sensory-event
    └─ Label/plate_cleaning

  combing
    ├─ Sensory-event
    └─ Label/combing

  pizza_cutting
    ├─ Sensory-event
    └─ Label/pizza_cutting

  pick_and_place
    ├─ Sensory-event
    └─ Label/pick_and_place

```
## Paradigm-Specific Parameters

- **Detected paradigm**: motor_imagery
- **Imagery tasks**: elbow_flexion, drawer, soup, weight_lifting, door, plate_cleaning, combing, pizza_cutting, pick_and_place
- **Cue duration**: 5.0 s
- **Imagery duration**: 5.0 s

## Data Structure

- **Trials**: 330
- **Trials context**: 15 runs of 24 trials each (4 rest + 4 elbow + 2 each of 8 goal tasks). Total: 60 rest + 30 per MI task = 330.

## Preprocessing

- **Data state**: raw
- **Preprocessing applied**: False

## Signal Processing

- **Classifiers**: LDA, DAL
- **Feature extraction**: bandpower, CSP, FBCSP
- **Frequency bands**: bandpass=[6.0, 35.0] Hz; mu=[7.0, 13.0] Hz; beta=[13.0, 30.0] Hz
- **Spatial filters**: CSP, FBCSP

## Cross-Validation

- **Method**: 5x5-fold
- **Folds**: 5
- **Evaluation type**: within_subject

## BCI Application

- **Applications**: motor_control, rehabilitation
- **Environment**: laboratory
- **Online feedback**: False

## Tags

- **Pathology**: Healthy
- **Modality**: Motor
- **Type**: Research

## Documentation

- **DOI**: 10.1371/journal.pone.0188293
- **License**: CC BY 4.0
- **Investigators**: Xin Zhang, Xinyi Yong, Carlo Menon
- **Senior author**: Carlo Menon
- **Institution**: Simon Fraser University
- **Department**: School of Engineering Science
- **Country**: CA
- **Repository**: Figshare
- **Data URL**: https://doi.org/10.6084/m9.figshare.5579461.v1
- **Publication year**: 2017
- **Keywords**: motor imagery, upper limb, elbow, BCI, EEG, kinesthetic imagery

## References

X. Zhang, X. Yong, and C. Menon, "Evaluating the versatility of EEG models generated from motor imagery tasks: An exploratory investigation on upper-limb elbow-centered motor imagery tasks," PLoS ONE, vol. 12, no. 11, e0188293, 2017. DOI: 10.1371/journal.pone.0188293
Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Hochenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A. and Jas, M. (2019). MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis. Journal of Open Source Software 4: (1896). https://doi.org/10.21105/joss.01896

Pernet, C. R., Appelhoff, S., Gorgolewski, K. J., Flandin, G., Phillips, C., Delorme, A., Oostenveld, R. (2019). EEG-BIDS, an extension to the brain imaging data structure for electroencephalography. Scientific Data, 6, 103. https://doi.org/10.1038/s41597-019-0104-8

---
Generated by MOABB 1.5.0 (Mother of All BCI Benchmarks)
https://github.com/NeuroTechX/moabb
