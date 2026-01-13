## Speech Emotion Recognition using Wav2Vec2 (Course Project)

This project applies transfer learning using a pretrained Wav2Vec2 model
for speech emotion recognition.

### Task
- Audio emotion classification (8 classes)

### Dataset
- RAVDESS

### Model
- Wav2Vec2 pretrained model
- Feature extractor frozen during initial training

### Training Strategy
- Audio padding and truncation
- Data augmentation (noise injection, time shifting)
- Weighted loss to address class imbalance
- Learning rate scheduling
- Fine-tuning on full dataset

### Results
- Validation Accuracy: ~96%

### References
- Baevski et al., wav2vec 2.0
- Hugging Face Transformers Documentation
