# StressECGNet A-Transformer-Driven-Network-for-Stress-Detection-from-Single-Lead-ECG-Signals
Stress is the body’s adaptive reaction to psychological or physiological threats, manifesting through several physical, behavioral, and emotional reactions. The conventional stress assessment methods that rely on handcrafted features or converted signal images are often subjective and error-prone; hence, underscoring the necessity for an automated stress detection framework to minimize stress-related health issues. In this study, we have proposed a novel model that integrates a transformer encoder with a convolutional neural network and a bidirectional long short-term memory architecture that detects stress from raw electrocardiogram signals. Two publicly available datasets, WESAD and Vollmer, are used to evaluate the proposed model. Our proposed approach shows an F1 score of 93.9%, an accuracy of 94.7%, a recall of 94.0%, and a precision of 94.4% on the WESAD dataset. On the Vollmer dataset, the model demonstrates an 88.1% F1 score, 88.2% accuracy, 88.2% recall, and 88.1% precision. To enhance the trustwortness of the model, we have proposed two novel explainability methods analysing the temporal and frequency components of the signal. Furthermore, the model was deployed on a resource-constrained device to evaluate its practical implementability. The experimental results, along with the model interpretability, demonstrate its robustness and generalizability, making it well- suited for sensor-based wearable healthcare and consumer devices in automatic stress detection.

<img width="1930" height="737" alt="SLettersModel" src="https://github.com/user-attachments/assets/97eaad9d-0fb3-49f0-a51c-9226d9870dfa" />

Fig. 1. The schematic diagram of (a) the structure of the proposed model, StressECGNet


# The Proposed Explainability Methods
## Segment-wise Perturbation-Based Attribution 
<img width="452" height="283" alt="image" src="https://github.com/user-attachments/assets/ca134017-a9f1-4a7f-afd1-6a2aec4081e1" /> 

<img width="417" height="287" alt="image" src="https://github.com/user-attachments/assets/a64a6271-ba47-4606-b08a-efafd46b0ac2" />

Fig. 2. Average perturbation-based attribution for (a) non-stressed and (b) stressed classes of a randomly selected subject (Subject 2, WESAD dataset), illustrating class-wise temporal importance of ECG signal segments.




## Integrated Gradients-Based Frequency Band Attribution 
<img width="455" height="370" alt="image" src="https://github.com/user-attachments/assets/afd6a744-6cda-42d4-8524-d0877ef947e5" /> 
<img width="3000" height="1050" alt="ECG_normal_ig_heatmap_conv" src="https://github.com/user-attachments/assets/82adc7ab-44bc-4d28-b9fd-e7a6d8bae9e2" />
Fig. 3.  Frequency band-wise integrated gradients attribution for a randomly chosen subject (Subject 2, WESAD dataset), indicating that the band 2 (4–8 Hz) and band 3 (8–13 Hz) frequency bands have the highest impact on the model’s decision-making process.

--end--

