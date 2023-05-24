# Multiclass Arrhythmia Detection and Classification from Photoplethysmography Signals Using a Deep Convolutional Neural Network


# Abstract
**Background** Studies have reported the use of photoplethysmography (PPG) signals to detect atrial fibrillation; however, the use of PPG signals in classifying multiclass arrhythmias has rarely been reported. Our study investigated the feasibility of using PPG signals and a deep convolutional neural network (DCNN) to classify multiclass arrhythmia types. **Methods and Results** Electrocardiogram (ECG) and PPG signals were collected simultaneously from a group of patients who underwent radiofrequency ablation for arrhythmias. A DCNN was developed to classify multiple rhythms based on 10-s PPG waveforms. Classification performance was evaluated by calculating the area under the microaverage receiver operating characteristic curve (microaverage AUC), overall accuracy, sensitivity, specificity, and positive and negative predictive values against annotations on the rhythm of arrhythmias provided by two cardiologists consulting the ECG results. A total of 228 patients were included; 118 217 pairs of 10-s PPG and ECG waveforms were employed. When validated against an independent test data set (23 384 PPG waveforms from 45 patients), the DCNN achieved an overall accuracy of 85.0% for six rhythm types (sinus rhythm, premature ventricular contraction, premature atrial contraction, ventricular tachycardia, supraventricular tachycardia, and atrial fibrillation); the microaverage AUC was 0.978; the average sensitivity, specificity, and positive and negative predictive values were 75.8%, 96.9%, 75.2%, and 97.0%, respectively. **Conclusions** This study demonstrated the feasibility of classifying multiclass arrhythmias from PPG signals using deep learning techniques. The approach is attractive for population-based screening and may hold promise for the long-term surveillance and management of arrhythmia.
![](https://github.com/zdzdliu/PPGArrhythmiaDetection/edit/main/fig1.png)

# Environment

Python 3.7.5, PyTorch 1.2.0

If you find the idea useful or use this code in your own work, please cite our [paper](https://www.ijcai.org/proceedings/2019/0816.pdf) as
```
@inproceedings{hong2019mina,
  title={{MINA:} Multilevel Knowledge-Guided Attention for Modeling Electrocardiography Signals},
  author={Hong, Shenda and Xiao, Cao and Ma, Tengfei and Li, Hongyan and Sun, Jimeng},
  booktitle = {IJCAI 2019},
  pages={5888--5894}
}
```

# Dataset

**Data** Training data can be found at https://archive.physionet.org/challenge/2017/#challenge-data

**Label** Please use Revised labels (v3) at https://archive.physionet.org/challenge/2017/REFERENCE-v3.csv

**Preprocessed** Or you can download my preprocessed dataset challenge2017.pkl from https://drive.google.com/drive/folders/1AuPxvGoyUbKcVaFmeyt3xsqj6ucWZezf
