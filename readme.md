# Potato & Tomato Leaf Disease Detection

<p align="center">
  <img src="https://img.shields.io/badge/AI-Computer%20Vision-blue?style=for-the-badge" alt="Computer Vision" />
  <img src="https://img.shields.io/badge/Framework-TensorFlow-orange?style=for-the-badge" alt="TensorFlow" />
  <img src="https://img.shields.io/badge/ML-SVM%20%2B%20CNN-green?style=for-the-badge" alt="Machine Learning" />
  <img src="https://img.shields.io/badge/Project-Plant%20Disease%20Detection-red?style=for-the-badge" alt="Plant Disease Detection" />
</p>

A high-impact computer vision project designed to detect diseases on potato and tomato leaves using image processing, classical machine learning, and deep learning.

## Why this project matters

Crop diseases can cause major agricultural losses. This project demonstrates a practical approach to automated plant disease recognition by analyzing leaf images and classifying them into healthy and diseased states.

The notebook compares several models to find the most effective approach for disease classification using a real plant image dataset.

## Project highlights

- disease classification for potato and tomato leaves
- comparison of handcrafted ML and deep learning models
- image preprocessing and segmentation pipeline
- transfer learning using MobileNetV2
- interactive Gradio app for quick inference
- results-focused notebook designed for experimentation and learning

## Results summary

The notebook reported the following performance on the selected disease classes:

| Model | Accuracy | Result |
|---|---:|---|
| SVM | 98.10% | Best classical machine learning performance |
| Random Forest | 98.10% | Same accuracy as SVM |
| CNN | 96.21% | Strong deep learning baseline |
| MobileNetV2 (fine-tuned) | 94.31% | Strong transfer learning result |

### Key takeaway

The handcrafted feature pipeline with traditional classifiers performed exceptionally well, reaching 98.10% accuracy. This shows that for this dataset, carefully engineered visual features can rival or outperform a standard deep learning approach when the task is well-structured and the classes are distinct.

## What is included

- image preprocessing: resizing, blur, HSV conversion, histogram enhancement
- segmentation: Canny edges, HSV thresholding, K-means clustering
- feature extraction: color, texture, and shape descriptors
- machine learning: SVM and Random Forest
- deep learning: custom CNN training
- transfer learning: MobileNetV2 fine-tuning
- user interface: Gradio-based prediction demo

## Repository structure

- `Computer_vision_Ahmed_Kallel.ipynb` — complete project notebook with data processing, training, and evaluation
- `readme.md` — project overview and usage guide

## Dataset

This project uses the PlantVillage dataset downloaded from Kaggle. A valid Kaggle account and a `kaggle.json` token are required to access the data.

## Recommended environment

This project was built primarily for Google Colab due to:

- `files.upload()` usage
- `/content` dataset paths
- direct Kaggle dataset download commands
- GPU-friendly deep learning workflow

A local Python environment is possible, but it may require path and dependency adjustments.

## Requirements

Install the following packages if running outside Colab:

- TensorFlow
- OpenCV
- scikit-image
- scikit-learn
- matplotlib
- seaborn
- Gradio
- kaggle

## How to run

1. Open the notebook in Google Colab.
2. Upload your Kaggle API token as `kaggle.json`.
3. Run the cells in sequence.
4. The notebook will:
   - download the dataset
   - prepare selected classes
   - preprocess leaf images
   - extract features
   - train SVM, Random Forest, CNN, and MobileNetV2 models
   - evaluate accuracy and classification reports
   - generate plots
   - launch a Gradio app for prediction

## Example workflow

```python
# Example from the notebook
# train model -> evaluate accuracy -> compare models -> predict new images
```

## Practical value

This project is useful for:

- plant disease monitoring
- AI-powered agricultural decision support
- educational learning in computer vision
- prototype development for smart farming systems

## Notes

- This is a research and demonstration project, not a production-grade deployment system.
- Training speed depends heavily on GPU availability.
- Local execution may need path modifications for the dataset and model outputs.
- The project is best suited for experimentation, teaching, and prototyping.

## Suggested next improvements

- add a proper `requirements.txt`
- split the notebook into reusable Python modules
- save trained models to disk
- create a dedicated inference script
- add deployment-ready app packaging
- document the exact disease classes and labels used
- add a license file for publication

## Conclusion

This is a strong and well-structured computer vision project with excellent experimental results. Reaching 98.10% accuracy using SVM and Random Forest demonstrates that the approach is both practical and effective. The project successfully combines classical image analysis, modern deep learning, and an interactive prediction interface in one compelling notebook.

The repository is already a solid proof of concept and is well positioned for further development into a full plant-disease recognition product.
