Saliency Prediction and Evaluation - README
===========================================

This project evaluates visual saliency prediction using two different models:
1. DeepGaze I (classic attention model)
2. SalFBNet (FBNet-based custom deep learning model)

Prepared as part of Assignment 3: "Saliency Prediction and Evaluation".


────────────────────────────────────────────
📁 Required Dataset:
────────────────────────────────────────────
Both notebooks require the dataset: `Saliency4asd.zip` with the following structure:

  Saliency4asd/
  ├── Images/
  ├── TD_FixPts/
  ├── ASD_FixPts/

Fixation point maps are used to generate fixation maps (FixMaps) used for saliency evaluation.


────────────────────────────────────────────
📘 1. Saliency using DeepGaze I.ipynb (DeepGaze I)
────────────────────────────────────────────
This notebook loads DeepGaze I, a pretrained saliency prediction model, and evaluates it using human fixation data.

Steps performed:
- Upload and extract `Saliency4asd.zip`
- Convert `*_FixPts` into `*_FixMaps`
- Predict saliency maps using DeepGaze I
- Evaluate with AUC-Judd, AUC-Shuffled, and NSS metrics

To run:
1. Open `Saliency using DeepGaze I.ipynb` in Google Colab by using this link-https://colab.research.google.com/drive/1H1Vp03j6YE8aULZxriL8uGSRhC1NJJCA?usp=sharing

2. Upload `Saliency4asd.zip` when prompted
3. Run all cells in order
4. Final results are printed for both TD and ASD groups


────────────────────────────────────────────
📘 2. SalFBNet.ipynb (FBNet-based model)
────────────────────────────────────────────
This notebook uses a custom FBNet-based deep neural network for saliency prediction.

Steps performed:
- Load and preprocess dataset
- Build and compile the SalFBNet model
- Train on available saliency data
- Predict and visualize saliency maps
- Compute evaluation metrics

To run:
1. Open `SalFBNet.ipynb` in Google Colab
2. Upload or link your training data and saliency ground truth
3. Train the model (ensure GPU runtime is enabled)
4. Evaluate and visualize outputs


────────────────────────────────────────────
📈 Output:
────────────────────────────────────────────
- Visual comparison of saliency predictions
- Metric scores for TD and ASD fixation agreement
- Model training curves (for SalFBNet)

────────────────────────────────────────────
📩 Contact:
────────────────────────────────────────────
Prepared by: 
1. Fabiha Tazri Okita 2425385650
fabiha.okita.242@northsouth.edu

2.Sabiha Hossain 2517115650
sabiha.hossain.251@northsouth.edu 

Group-2
Assignment: CSE 532 - Advanced Computer Architecture


