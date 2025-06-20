# Early-Identification-of-dysgraphia-using-image-processing

📌 Project Description
Dysgraphia is a neurological learning disability that affects handwriting and fine motor skills. Early detection is crucial for providing support to affected individuals.

This project automates the classification of handwriting samples into:

 Normal (Label: 0)

Dysgraphia (Reversal) (Label: 1)

The model is trained using extracted image features and predicts whether a handwriting sample shows signs of dysgraphia.

📁 Dataset Structure
Your dataset should consist of images organized into two folders:
/Normal       → Contains normal handwriting samples
/Reversal     → Contains samples with reversal errors (Dysgraphia indicator)
Each folder can contain subfolders or be a direct collection of .png, .jpg, etc.

🧪 Features Extracted from Images
For each image:

Mean intensity – Average pixel brightness (grayscale)

Standard deviation – Contrast level

Edge count – Number of detected edges (Canny edge detection)

These features are used to train the AdaBoost classifier.

🛠️ Technologies Used
Python 3.x

OpenCV

NumPy

Scikit-learn (AdaBoostClassifier)

Matplotlib

Joblib (for model saving/loading)

Google Colab or Jupyter (recommended)

🚀 How to Run
1. Model Training
Modify the paths to your dataset in the script.

Run the script to:

Extract features

Train AdaBoost classifier

Display accuracy and confusion matrix

Save the trained model as .pkl

2. Testing on a New Image
Load the saved model

Upload a handwriting image sample

Extract features and make prediction

Display the prediction result with the image

📊 Output Example
Training accuracy printed

Confusion matrix visualized

Bar chart for model accuracy

Image preview with title: Predicted: Normal or Predicted: Dysgraphia

💡 Use Cases and Benefits
Early screening tool in schools or clinics

Can be used in mobile apps for parental assessment

Promotes awareness and early intervention for learning disabilities

Valuable for education researchers and special educators

✅ Future Improvements
1.Use deep learning models (e.g., CNNs) for better accuracy

2.Expand dataset for generalization

3.Improve feature extraction (slant, spacing, pressure analysis)
