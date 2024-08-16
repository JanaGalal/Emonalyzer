# Arabic Speech Emotion Recognition Project

## Overview

This project focuses on developing an Arabic Speech Emotion Recognition (SER) system using advanced techniques and models. The core of this project is based on the `ellgeish/wav2vec2-large-xlsr-53-arabic` model from Hugging Face, integrated with additional techniques to enhance performance and accuracy.

## Dataset

### Datasets Used

- **EYASE Dataset**: Contains 579 utterances with four emotional states: Sad, Happy, Angry, Neutral.
- **EAED Dataset**: Contains 3164 records with six emotional states, including Surprise and Fear.

### Data Processing

- **Data Preparation**: Audio files are organized in a directory format, named with the pattern `MAL_AsserYassin_ang_2646.wav`.
- **Balancing Classes**: Implemented data augmentation techniques to balance the number of records for the "happy" and "angry" emotions.

## Workflow

### Data Import and Splitting

- Imported data from Google Drive into Kaggle.
- Split data into training, validation, and test sets with stratification to maintain the proportion of each emotion category.

### Model Training

- Utilized the `ellgeish/wav2vec2-large-xlsr-53-arabic` pretrained model from Hugging Face.
- Applied fine-tuning on the Arabic SER dataset to predict the four primary emotions: Happy, Sad, Angry, and Neutral.
- Achieved a 72% accuracy after 7 epochs of training.

### Model Evaluation

- Evaluated model performance using metrics such as accuracy and F1-score.
- Employed techniques to address class imbalance by weighting classes differently in the loss function.

## Results

- **Accuracy**: Achieved 72% accuracy in emotion classification.
- **Model Performance**: Significant improvement noted compared to models built from scratch.
- **Class Imbalance Handling**: Implemented different weighting strategies for minority classes to improve overall model performance.

## Conclusions

- The use of the Wav2Vec2 model significantly enhanced the performance of the Arabic Speech Emotion Recognition system.
- Balancing class distribution through data augmentation and weighting strategies proved effective in improving classification accuracy.
- Further improvements could involve expanding the model to recognize additional emotions and exploring other advanced techniques for real-time processing.

## Future Work

- **Expansion**: Extend the model to include additional emotions (e.g., Surprise, Fear) from the EAED dataset.
- **Real-Time Processing**: Optimize the model for real-time emotion recognition.
- **Integration**: Explore the integration of multimodal features for improved accuracy.
