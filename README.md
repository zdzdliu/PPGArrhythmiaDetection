# Multiclass Arrhythmia Detection and Classification from Photoplethysmography Signals Using a Deep Convolutional Neural Network
This repository contains code and dataset for the paper “Multiclass Arrhythmia Detection and Classification from Photoplethysmography Signals Using a Deep Convolutional Neural Network”

## Abstract
**Background** 
Studies have reported the use of photoplethysmography (PPG) signals to detect atrial fibrillation; however, the use of PPG signals in classifying multiclass arrhythmias has rarely been reported. Our study investigated the feasibility of using PPG signals and a deep convolutional neural network (DCNN) to classify multiclass arrhythmia types. **Methods and Results** 
Electrocardiogram (ECG) and PPG signals were collected simultaneously from a group of patients who underwent radiofrequency ablation for arrhythmias. A DCNN was developed to classify multiple rhythms based on 10-s PPG waveforms. Classification performance was evaluated by calculating the area under the microaverage receiver operating characteristic curve (microaverage AUC), overall accuracy, sensitivity, specificity, and positive and negative predictive values against annotations on the rhythm of arrhythmias provided by two cardiologists consulting the ECG results. A total of 228 patients were included; 118 217 pairs of 10-s PPG and ECG waveforms were employed. When validated against an independent test data set (23 384 PPG waveforms from 45 patients), the DCNN achieved an overall accuracy of 85.0% for six rhythm types (sinus rhythm, premature ventricular contraction, premature atrial contraction, ventricular tachycardia, supraventricular tachycardia, and atrial fibrillation); the microaverage AUC was 0.978; the average sensitivity, specificity, and positive and negative predictive values were 75.8%, 96.9%, 75.2%, and 97.0%, respectively.
**Conclusions** This study demonstrated the feasibility of classifying multiclass arrhythmias from PPG signals using deep learning techniques. The approach is attractive for population-based screening and may hold promise for the long-term surveillance and management of arrhythmia.

![](https://github.com/zdzdliu/PPGArrhythmiaDetection/blob/main/fig1.png)

## Dataset

The validation set and test set are provided in .mat format, with each .mat file representing an individual. The information enclosed within each .mat file is as follows:

ppgseg: ppg segments, each with a length of 10s (sampling rate =100Hz)
labels: labels (range 0 to 5) corresponding to ppg signal segments

0 sinus rhythm
1 premature ventricular contraction
2 premature atrial contraction
3 ventricular tachycardia
4 supraventricular tachycardia
5 atrial fibrillation


## Citation

If you use this repository, part or all of the full dataset, and/or our paper as part of your research, please cite the [publication](https://www.ahajournals.org/doi/10.1161/JAHA.121.023555) as follows:
```
@article{liu2022multiclass,
  title={Multiclass Arrhythmia Detection and Classification From Photoplethysmography Signals Using a Deep Convolutional Neural Network},
  author={Liu, Zengding and Zhou, Bin and Jiang, Zhiming and Chen, Xi and Li, Ye and Tang, Min and Miao, Fen},
  journal={Journal of the American Heart Association},
  volume={11},
  number={7},
  pages={e023555},
  year={2022},
  publisher={Am Heart Assoc}
}
```
