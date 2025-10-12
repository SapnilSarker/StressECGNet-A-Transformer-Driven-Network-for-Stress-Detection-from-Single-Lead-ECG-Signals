# StressECGNet A-Transformer-Driven-Network-for-Stress-Detection-from-Single-Lead-ECG-Signals
Stress is the body's adaptive reaction to psychological or physiological threats, expressed as several physical, behavioral, and emotional responses. The conventional stress assessment methods are often subjective and error-prone; hence, an automated stress detection protocol is needed to minimize stress-related health issues. In this study, we have proposed a novel transformer encoder-based convolutional neural network-bidirectional long short-term memory model that detects stress using raw electrocardiogram signals. Two publicly available datasets, WESAD and Vollmer, are used to evaluate the proposed model. Our proposed approach shows an F1 score of 93.9%, an accuracy of 94.7%, a recall of 94.0%, and a precision of 94.4% on the WESAD dataset. On the Vollmer dataset, the model demonstrates an 88.1% F1 score, 88.2% accuracy, 88.2% recall, and 88.1% precision. To the best of our knowledge, these results surpass the state-of-the-art ECG signal-based subject-independent stress detection techniques. The experimental results and model interpretability of this study show the robustness and generalizability of the proposed model, with its potential implementation in wearable technologies.

<img width="1930" height="737" alt="SLettersModel" src="https://github.com/user-attachments/assets/97eaad9d-0fb3-49f0-a51c-9226d9870dfa" />

**Fig. 1.** The schematic diagram of (a) the structure of the proposed model, StressECGNet

## Integrated Gradients-Based Frequency Band Attribution 
<img width="455" height="370" alt="image" src="https://github.com/user-attachments/assets/afd6a744-6cda-42d4-8524-d0877ef947e5" />

<img width="3000" height="1050" alt="ECG_normal_ig_heatmap_conv" src="https://github.com/user-attachments/assets/82adc7ab-44bc-4d28-b9fd-e7a6d8bae9e2" />
**Fig. 1.** Frequency band-wise integrated gradients attribution for a randomly chosen subject (Subject 2, WESAD dataset), indicating that the band 2 (4–8 Hz) and band 3 (8–13 Hz) frequency bands have the highest impact on the model’s decision-making process.


**transformer-vollmer.ipynb contains the code that has been used for the LOOCV evaluation of the Vollmer dataset.**


**transformer-wesad.ipynb contains the code that has been used for the LOOCV evaluation of the WESAD dataset.**


**model interpretability file is for t-SNE representation of different model layers**


**StressECGNet_model file is the code of the overall model representation**


#DataAugmentation file is the code of applied minority class data augmentation techniques.
