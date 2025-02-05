# Plant Disease Classification using Deep Learning 🌿🦠
# This repository contains a deep learning-based image classification model for detecting plant diseases using TensorFlow/Keras. The model is trained on a dataset of labeled plant images and predicts the plant type and the specific disease affecting it.

Features
✅ Image Preprocessing & Augmentation: Resizes and normalizes images for model input.
✅ Deep Learning Model: Uses a CNN trained on a labeled dataset.
✅ Accurate Predictions: Outputs the plant name, disease name, and confidence score.
✅ Detailed Class Probabilities: Displays the probability distribution across all classes.
✅ User-Friendly Output: Clearly states the identified plant, disease, and confidence level.

Installation Steps
Follow these steps to set up and run the model:

1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/plant-disease-classification.git
cd plant-disease-classification
2. Set Up a Virtual Environment (Optional but Recommended)
bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
(Ensure requirements.txt includes TensorFlow, NumPy, Pillow, etc.)

4. Download Pre-Trained Model (If Required)
If the model is pre-trained, download the weights and place them in the models/ directory:

bash
Copy
Edit
mkdir models
wget -O models/plant_disease_model.h5 "YOUR_MODEL_DOWNLOAD_LINK"
5. Run Prediction
bash
Copy
Edit
python predict.py --image /path/to/your/image.jpg
Example Output
yaml
Copy
Edit
Identified Plant: Pepper__bell  
Detected Disease: Bacterial_spot  
Confidence Score: 97.04%  

Class Probabilities:  
Pepper__bell___Bacterial_spot: 97.04%  
Pepper__bell___healthy: 0.06%  
Potato___Early_blight: 0.75%  
Tomato_Early_blight: 1.99%  
...  

According to our Confidence Score, the disease is: Bacterial_spot
Requirements
Python 3.7+
TensorFlow / Keras
NumPy
PIL (Pillow)
