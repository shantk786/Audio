EMERGENCY VEHICLE DETECTION AND TRAFFIC SIGNAL CONTROL

This project uses a CNN-based deep learning model to detect emergency vehicle sirens and automatically update traffic signals accordingly. The system can identify ambulance, fire truck, and police sirens from audio recordings and adjust traffic lights in real time to provide a clear path for emergency responders.

🔧 How It Works

Audio Input: The system takes an audio file as input.

Feature Extraction: The trained model uses MFCC (Mel-Frequency Cepstral Coefficients) to process audio.

Prediction: The CNN model classifies the audio into categories:

🚑 Ambulance
🚒 Fire Truck
🚓 Police
🚗 Noise (No emergency)

Traffic Signal Update: If an emergency vehicle is detected:
An examplefile is created to show that
The traffic light in its direction turns GREEN.
All other signals turn RED for 5 seconds before resetting.


Model Details

Architecture: Convolutional Neural Network (CNN)
Features: Extracted using MFCC
Labels: One-hot encoding of vehicle types
Dataset: Includes siren sounds for various emergency vehicles
