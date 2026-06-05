# HyzeACR (Astronomical Character Recognition)

An Image Classification model that detects galaxies, moons, planets, and nebulaes using TensorFlow and Keras

---

## 🚀 Live Demo
Go to https://hyzeacr.netlify.app
---

## 🧠 What This Project Does

This AI system classifies space related images into the following categories:

- 🌕 Moon  
- 🪐 Planet  
- 🌌 Galaxy  
- ☁️ Nebula  

It supports:
- Image based classification
---

## ⚙️ How It Works

1. A trained machine learning model is loaded in the browser using TensorFlow.js
2. Any image of a Moon, Planet, Nebulae, or a Galaxy is uploaded to the model
3. The model predicts the most likely space object  
4. The predictions are displayed

---

## How to use

1. The easiest way to use the model is by using the web demo at https://hyzeacr.netlify.app (The model is hosted with Google Cloud)
2. Install a local TensorFlow environment
3. Run this command pip install tensorflow numpy
4. Next write a python script to run the model
5. Here is an example "import numpy as np
from tensorflow.keras.models import load_model

# 1. Load the local .h5 model file
model_path = 'model.h5'
model = load_model(model_path)
print("Model loaded successfully!")

# 2. Prepare your dummy or real data 
# (Replace this with your actual preprocessed input data)
# Example: If your model expects a 2D image of 28x28 pixels with 1 color channel:
input_shape = model.input_shape  # Check what dimensions the model expects
print(f"Expected input shape: {input_shape}")

# Generate sample random data matching the expected shape
# Typically: (batch_size, height, width, channels)
sample_input = np.random.rand(1, 28, 28, 1) 

# 3. Run inference
predictions = model.predict(sample_input)

# 4. Output the result
print("Inference results:")
print(predictions)
"

---

## 🧪 Tech Stack

- TensorFlow.js (browser inference)
- Keras (model training)
- TensorFlow (ML framework)
- JavaScript (frontend logic)
- HTML (UI)

---
## Created by Hitesh Vinothkumar
