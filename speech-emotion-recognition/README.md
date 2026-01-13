## Speech Emotion Recognition using Wav2Vec2 (Course Project)

This project implements a speech emotion recognition system using
transfer learning with a pretrained Wav2Vec2 model.

This notebook was developed as part of a Deep Learning course assignment
and focuses on applying correct audio preprocessing and training practices.

---

### Task
- Speech emotion classification
- 8 emotion classes (neutral, calm, happy, sad, angry, fearful, disgust, surprised)

### Dataset
- RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)
- Audio-based emotion dataset
- Dataset accessed via Kaggle

### Model
- Wav2Vec2 pretrained model (`facebook/wav2vec2-base`)
- Feature extractor frozen during initial training
- Classification head fine-tuned for emotion recognition

### Training Strategy
- Audio resampling to 16 kHz
- Padding and truncation to fixed duration
- Data augmentation (noise injection, time shifting)
- Stratified train/validation split
- Weighted loss to handle class imbalance
- Learning rate scheduling
- Final fine-tuning on the full dataset

### Results
- Validation Accuracy: ~96%
- Strong per-class precision, recall, and F1-scores

### Notes
- This project is included as part of coursework documentation.
- The emphasis is on clean implementation and reproducibility.

---

## References

[1] A. Baevski et al., “wav2vec 2.0: A Framework for Self-Supervised Learning of Speech Representations,”  
NeurIPS 2020.  
https://arxiv.org/abs/2006.11477

[2] Livingstone, S. R., & Russo, F. A., “The Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS),”  
PLOS ONE, 2018.  
https://doi.org/10.1371/journal.pone.0196391

[3] Kaggle Dataset: *Speech Emotion Recognition (RAVDESS)*.  
https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio

[4] Hugging Face Transformers Documentation.  
https://huggingface.co/docs/transformers/model_doc/wav2vec2
