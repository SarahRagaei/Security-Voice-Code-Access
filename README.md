# Security Voice-code Access System
A voice-based authentication system that grants or denies access based on **voice recognition** and **spectrogram analysis**. It combines voice passcode recognition and speaker identification and performs authentication in real-time, providing instant feedback on access status.

## Features
### 1. Dual Operation Modes
It works in two distinct modes:

**Mode 1 – Security Voice Code:**
- Access is granted only if a user speaks one of the predefined *valid passcode* sentences: “Open middle door”, “Unlock the gate”, or “Grant me access”.

**Mode 2 – Security Voice Fingerprint:**
- Access is granted if the *valid passcode* sentence is spoken by one of the *pre-authorized* individuals.
- The system is trained on 8 different individuals.
- Admin can select which individuals are granted access via checkboxes.

### 2. Voice Recording
Users can start/stop recording voice input via the 🎙️microphone button.

### 3. Spectrogram Viewer
Displays spectrogram of the spoken voice-code in real time for visual analysis.

### 4. Analysis Summary
Presents a summary of the similarity analysis results, including:
- Pie chart showing how much the spoken sentence matches each of the 3 valid passcodes.
- Pie chart showing how much the spoken voice matches each of the 8 trained individuals.

### 5. Individual Authorization
Allows users to select which individuals among the trained 8 users are granted access.

### 6. Access Decision
A clear indicator for “Access Gained” or “Access Denied”.

### 7. User Interface
Intuitive user interface with clear controls for mode selection, voice recording, spectrogram visualization, and result display.


## Demo Screenshot
![1](image.png)


## How to Use
**1. Mode Selection:** Choose between Security Voice Code mode or Security Voice Fingerprint mode.

**2. Recording Voice-Code:** Click the button to start recording the voice-code.

**3. Spectrogram Viewer:** Visualize the spectrogram of the spoken voice-code.

**4. Analysis Results:** View a summary of the analysis results, including:
  * A Pie chart showing the match percentages for each of the predefined passcode sentences.
  * A Pie chart showing the match percentages for each of the stored individuals' voiceprints.

**5. Access Status:** Receive feedback on access status, either "Access gained" or "Access denied".

## Dependencies
- PyQt5
- sounddevice
- scipy
- numpy
- matplotlib
- librosa
- joblib
- python_speech_features

## Running The Project
1. Install dependencies:

```pip install PyQt5 sounddevice scipy numpy matplotlib librosa joblib python_speech_features
```

2. Run the application:

```python main.py```


