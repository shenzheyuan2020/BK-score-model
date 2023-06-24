Project Title
Introduction
B&K Score of ADC Prediction Using Graph Attention Network (GAT)


This project provides a Python script to predict the Bscore(PAMPA) and the Kscore(TOP1 pIC50) of molecules using a Graph Attention Network (GAT). The script uses RDKit and DeepChem libraries to featurize the molecules and predicts their properties using a pre-trained model. The predictions are then saved to an Excel file.


Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. This guide assumes the use of Ubuntu 20 or 22 as your operating system.



Installation
This project requires the following dependencies:

Python 3.7.16
RDKit 2022.9.5
PyTorch 1.13.1+cu116
PyTorch Geometric 2.3.0
torchaudio 0.13.1
torchvision 0.14.1
DGL 1.0.2+cu116
DGL-Life 0.3.2
DeepPhem 2.7.1
You can quickly set up the required environment using conda. We have provided a environment.yaml file to help you with this. Run the following command in your terminal:


conda env create -f environment.yaml
conda activate BKmodel
This will create a new conda environment with all the required dependencies installed.

Usage

The software does not require extra installation steps and can be run through jupyter notebook after installing the environment. Please make sure your machine has CUDA installed
Example of Predicting a New Molecule

You can also use the script to predict properties for a new molecule that you are interested in. Simply replace the SMILES representation of the example molecule with the one for your molecule, and run the script.

In the jupyter notebook, you can change the smiles list with your own and then run the cells one by one to make the prediction. The necessary input file is 'Your_own_prediction_data.xlsx'. 

Please refer to the file type of the PAMPA.xlsx that puts the smiles list in the smiles column."

The model will give the values of B score and K score for different molecules after prediction.

During the operation, please make sure the checkpoint file is under the same path as the jupyter file.

Contributing
If you are open to contributions, explain how others can contribute to your project. Include any style guides or testing frameworks you're using.

License
Inform users about the license under which you're releasing your project.

Feel free to customize this template to fit your project's needs. The more information you can provide about your project and how to use it, the more useful it will be to your users.