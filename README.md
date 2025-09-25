🌱 Plant Disease Classifier
🚀[ Try the Live Demo on Hugging Face Spaces!](https://huggingface.co/spaces/xiaolinouo/plant-disease-classifier) 🚀

(Please replace the link above with your final Hugging Face Space URL)
📌 Project Overview

I have developed an end-to-end deep learning application designed to rapidly diagnose plant health from a single leaf image. The model can identify 38 different classes of plant diseases and healthy states, providing an easy-to-use tool for early disease detection for gardeners and farmers alike.

This project was more than just model training; it was a deep dive into the practical challenges of deployment. I troubleshooted and overcame several low-level technical hurdles in the PyTorch model quantization and deployment pipeline, such as state_dict mismatches and aten::add.out operator incompatibilities. Ultimately, I successfully packaged a high-performance PyTorch model into a stable, interactive web application.
✨ Key Features & Highlights

    End-to-End Pipeline: Fully implemented the entire workflow from data augmentation and model fine-tuning (ResNet-50) to final web deployment using Flask.

    High Accuracy: The original floating-point model achieved 99% accuracy on the PlantVillage dataset, ensuring reliable diagnoses.

    Interactive Web App: Features a clean, user-friendly interface that allows users to easily upload an image and receive an instant diagnosis along with relevant solution information.

    Successfully Deployed: The project is live on Hugging Face Spaces, providing a public online demo that showcases my practical MLOps skills.

    Future-Ready (RAG Integration): The next phase of the project is to integrate a RAG (Retrieval-Augmented Generation) system, upgrading the application from a simple "identification tool" to an "intelligent diagnostic expert" capable of more intelligent, contextual interactions.

🛠️ Tech Stack

    Backend: Python, PyTorch (for deep learning), Flask (for web server)

    Model: Fine-tuned ResNet-50 pre-trained on ImageNet

    Deployment: Docker, Hugging Face Spaces

    Dataset: PlantVillage Dataset

📂 Project Structure

The structure in the Hugging Face repository is the final, deployment-optimized version:

/
├── app.py                     # Main Flask application
├── best_model.pth             # The final, fine-tuned floating-point model
├── class_names.json           # List of class names
├── Solution.json              # Disease solution data
├── Dockerfile                 # Hugging Face deployment configuration
├── requirements.txt           # Python dependencies
├── static/                    # Static files (CSS, JS, uploaded images)
│   └── uploads/
└── templates/                 # HTML templates
    ├── index.html
    └── result.html

⚙️ How to Run Locally

    Clone the repository:

    git clone [https://github.com/](https://github.com/)[your-username]/[your-repo-name].git
    cd [your-repo-name]

    (Please replace [your-username] and [your-repo-name])

    Create a virtual environment (recommended):

    python -m venv venv
    source venv/bin/activate  # On macOS/Linux
    venv\Scripts\activate   # On Windows

    Install dependencies:

    pip install -r requirements.txt

    Download the model:
    Due to its size, the model file is not included in the Git repository. Please download best_model.pth from the link below and place it in the project's root directory.

    Download Model (best_model.pth) from Google Drive：https://drive.google.com/file/d/1MgBPD5wfl_j3VyBDyShRfIGNcIyYgpH9/view?usp=drive_link

    Recommendation: For better version control and community access, consider uploading the model to the Hugging Face Hub in the future.

    Run the Flask application:

    python app.py
