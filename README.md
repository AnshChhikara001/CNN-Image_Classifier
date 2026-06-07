🧠 CNN Image Classifier — CIFAR-10
A Convolutional Neural Network built from scratch using PyTorch to classify images across 10 categories from the CIFAR-10 dataset.

📌 Classes
airplane · automobile · bird · cat · deer · dog · frog · horse · ship · truck

🏗️ Model Architecture
Input (3 × 32 × 32)
    ↓
Conv2d(3 → 32) + ReLU + MaxPool
    ↓
Conv2d(32 → 64) + ReLU + MaxPool
    ↓
Conv2d(64 → 128) + ReLU + MaxPool
    ↓
Flatten
    ↓
Linear(2048 → 256) + ReLU
    ↓
Linear(256 → 10)

📉 Training Results
EpochLoss10.842830.576950.380270.2352100.1216

Trained for 10 epochs using Adam optimizer and CrossEntropyLoss. Loss decreased from 0.84 → 0.12.


⚙️ Setup & Run
1. Clone the repo
bashgit clone https://github.com/AnshChhikara001/CNN-Image-Classifier.git
cd CNN-Image-Classifier
2. Install dependencies
bashpip install torch torchvision
3. Run the notebook
Open CNN_Image-Classification.ipynb in Jupyter and run all cells. The CIFAR-10 dataset (~170MB) will be downloaded automatically.

🛠️ Tech Stack

Python 3.x
PyTorch
torchvision
Jupyter Notebook


📁 Project Structure
CNN-Image-Classifier/
│
├── CNN_Image-Classification.ipynb   # Main notebook
├── requirements.txt                 # Dependencies
└── README.md                        # This file

🔮 Future Improvements

 Add Dropout layers for regularization
 Experiment with Batch Normalization
 Add data augmentation (flips, crops)
 Plot loss curve with matplotlib
 Try transfer learning with ResNet


👤 Author
Ansh Chhikara — @chikaraansh0@gmail.com
