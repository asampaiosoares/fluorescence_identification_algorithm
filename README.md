# fluorescence_identification_algorithm

This is a guide on how to use the provided Jupyter Notebook to train a fluorescence identification algorithm using FastAI and ResNet34. The notebook contains cells that load a dataset, create a data block, train the algorithm, fine-tune it, and export the model.
Requirements

    Python 3.9.7
    FastAI
    Jupyter Notebook
    torchvision (for ResNet34)

Instructions

    Install the required packages:

pip install fastai
pip install jupyter
pip install torchvision

    Start Jupyter Notebook:

jupyter notebook

    Open the provided Notebook file.

    Update the DATASET_PATH variable in the second cell with the path to your dataset folder.

    Run each cell one by one, starting from the top. You can do this by selecting a cell and pressing Shift+Enter. Make sure to run them in the order they appear in the notebook.

    After running the last cell, your trained model will be saved as 'first.pth' in the current directory.

Notebook Overview

    Cell 1: Sets up compatibility for running the notebook on both Linux and Windows systems.
    Cell 2: Sets the path to your dataset folder.
    Cell 3: Loads the dataset and applies transformations for data augmentation.
    Cell 4: Initializes the ResNet34 model for training.
    Cell 5: (Optional) Finds the optimal learning rate for fine-tuning the model.
    Cell 6: Fine-tunes the model for 4 epochs.
    Cell 7: Outputs the confusion matrix for the trained model.
    Cell 8: Displays the top losses for the model.
    Cell 9: Exports the trained model as 'export.pkl' in the current directory.
    Cell 10: Saves the trained model as 'first.pth' in the current directory.

Once you have completed these steps, you should have a trained model that can be used for fluorescence identification.
