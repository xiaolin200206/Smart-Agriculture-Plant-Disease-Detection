📌 Project Overview

This project uses ResNet to classify plant leaf images into multiple categories (healthy and diseased).
The goal is to provide farmers with an easy-to-use tool for early plant disease detection, which can help reduce crop loss.

Dataset: PlantVillage Dataset

Framework: PyTorch

🚀 Features

🌿 Classifies plant leaf images into 11 classes

🔍 Based on ResNet for robust image classification

📊 Trained on 160k+ images from PlantVillage

🖥️ Deployment-ready (Flask / Streamlit support)

⚡ Supports model optimization (pruning, quantization in future)

📂 Project Structure
📁 plant-disease-detection
 ┣ 📂 dataset/            # dataset (not included in repo, link to Kaggle)
 ┣ 📂 models/             # trained model files (.pth)
 ┣ 📂 notebooks/          # Jupyter notebooks for training & testing
 ┣ 📂 app/                # Flask or Streamlit app
 ┣ 📄 requirements.txt    # dependencies
 ┣ 📄 README.md           # project documentation
 
⚙️ Installation
# Clone the repository
git clone https://github.com/yourusername/plant-disease-detection.git
cd plant-disease-detection

# Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

🧑‍💻 Usage
1. Train the model
python train.py

2. Run inference
python predict.py --image sample_leaf.jpg

3. Deploy with Streamlit
streamlit run app/app.py

📊 Results

Accuracy: 99%

Model: ResNet50 (pretrained on ImageNet, fine-tuned)

Training Time: about 2 hours on GPU
![training curve](train_curve.png)
![deploy_result](deploy_result.png)

📌 Future Work

✅ Add quantization & pruning for lightweight deployment

✅ Collect local datasets for better generalization

🔜 Deploy to AWS (EC2 + S3)

Download link:https://drive.google.com/file/d/1VKVLtOiuy8XgROLky_WoevOwEJudC3zw/view?usp=drive_link
