# Data Science Final Project

## Project Overview
The final project for this course provides an opportunity to apply the skills and knowledge gained throughout the course to a real-world problem in data science. This project is a significant component of your final grade and encourages collaboration in teams of up to three members, with individual contributions assessed.

## Assignment Objectives
- **Develop a Deep Learning Pipeline**: Create a robust pipeline for training and evaluating machine learning models.
- **Tune and Debug Models**: Experiment with different algorithms and techniques to optimize performance.
- **Engage in Real-Life Problem Solving**: Address a relevant issue in the field of data science, specifically focusing on drug-drug interaction (DDI) prediction.

## Project Requirements

### Project Proposal (Optional)
- **Title**: A concise statement of the problem and proposed solution.
- **Problem Definition**: Describe the problem, its significance, and the inputs and outputs of your system.
- **Dataset**: Identify a high-quality dataset, including its size and any necessary preprocessing steps.
- **Evaluation Metrics**: Define how the model's performance will be measured.
- **Baseline Method**: Describe a simple method for comparison.

### Final Report
The final report should encompass the following sections:
- **Abstract**: Briefly introduce the problem and the proposed solution.
- **Introduction**: Explain the problem and anticipated challenges.
- **Related Work/Background**: Summarize recent works that address similar issues.
- **Proposed Method**: Provide a thorough explanation of your approach, including preprocessing and model architecture.
- **Results**: Present the dataset used and describe experiments conducted, along with outcomes.
- **Discussion**: Analyze the effectiveness of your method, comparing it to other approaches.
- **References**: Cite all sources utilized in the project.

### Deliverables
- Write-up in PDF format.
- GitHub repository for project code and documentation.
- Jupyter notebook with reproducible experiments.
- Detailed description of each team member's responsibilities.
- Presentation: A 10-15 minute presentation showcasing the project, including:
  - Problem definition and significance.
  - Proposed solution and its applicability.
  - Justification of the deep learning approach.
  - Analysis of results and discussion of challenges faced.

## Project Implementation

### Team Members
- **Mehrdad Baradaran**
- **Katayoun Kobraei**

### Project Overview
In this project, we employed neural networks and deep learning techniques to tackle the problem of predicting side effects from drug combinations, focusing on Drug-Drug Interaction Prediction.

### Understanding Drug Interaction Data
We analyzed datasets containing comprehensive drug information and their interactions, including features like chemical structures, targets, enzymes, and known side effects.

### Addressing Data Challenges
The datasets posed challenges such as sparsity, imbalance, and incomplete information. We implemented strategies to overcome these issues, ensuring our models could learn effectively from the available data.

### Proposed Methodologies
1. **Approach 1**: Developed a dual-model neural network that combines an autoencoder for dimensionality reduction and a classifier for predicting side effects. This design aimed to mitigate data imbalance and enhance feature representation.
   
2. **Approach 2**: Introduced a method for calculating drug similarity using Jaccard similarity, aiding in feature extraction and improving prediction performance by leveraging similar drug properties.

3. **Approach 3**: Integrated the first two approaches to create a robust model that utilizes both advanced feature extraction and effective classification strategies.

### Evaluation and Results
We evaluated our models using various metrics (accuracy, precision, recall, F1 score, AUPRC, AUROC) to compare their performance against baseline methods like k-nearest neighbors (KNN). Our results demonstrated that the integrated approach significantly outperformed existing state-of-the-art models.

### Key Findings
- The combined approach successfully addressed issues of data imbalance and sparsity, leading to higher prediction accuracy and better interpretability of drug interactions.
- The results highlighted the importance of leveraging multiple data sources and advanced neural network architectures to improve DDI prediction.

### Future Directions
Future work could explore incorporating more extensive datasets, experimenting with different neural network architectures, and enhancing preprocessing techniques for better feature extraction.
