##  Setup Instructions  

### 1 Clone the Repository  
```bash
git clone https://github.com/bhavyajethi/deepfake-audio-detection.git
cd deepfake-audio-detection

### 2 Create a Virtual Environment (Optional but Recommended)
On macOS/Linux:
python3 -m venv venv
source venv/bin/activate

On Windows:
python -m venv venv
venv\Scripts\activate

### 3 Install Required Dependencies
pip install numpy pandas librosa matplotlib seaborn tqdm scikit-learn imbalanced-learn tensorflow resampy

***Dataset***
https://www.kaggle.com/datasets/birdy654/deep-voice-deepfake-voice-recognition
Download the dataset and extract it into the data/ directory within your project.

Expected Folder Structure:
data/
├── REAL/   # Contains real human voice audio files
├── FAKE/   # Contains deepfake-generated audio files

### 4 Running the Model
Run Feature Extraction & Training:
python train.py

### 5 Evaluate the Trained Model
python evaluate.py
