# JetBot Road Following by Regression

This is the instruction for **Road Following by Regression** exmaple in NCKU-NITKC AI Robotics Lab. 


## Setup
1. Log in to your JetBot from a web browser.
1. Open a terminal. Your current working directory must be `workspace` now. 
1. Then navigate to `workspace/jetbot/notebooks` directory.
    ```
    $ cd jetbot/notebooks
    ```
1. Clone this repository.
    ```
    $ git clone https://github.com/naoya1110/road_following_by_regression.git
    ```

## Data Collection
1. Navigate to `workspace/jetbot/notebooks/road_following_by_regression` directory in the file browser.
1. Open `data_collection.ipynb`
1. Perform data collection by following instructions in the notebook.
1. Download `dataset_reg.zip` to your local PC.

## Model Training
1. Open `train_model_resnet18.ipynb` in Google Colab from [here](https://colab.research.google.com/github/naoya1110/road_following_by_regression/blob/main/train_model_resnet18.ipynb)
1. Upload `dataset_reg.zip` by using the file browser in Google Colab.
1. Train a model by following instructions in the notebook.
1. Download `best_model_reg_resnet18.pth` to your local PC

## Build TensorRT Model
1. Open `build_resnet18_trt.ipynb`
1. Upload `best_model_reg_resnet18.pth` to `workspace/jetbot/notebooks/road_following_by_regression` directory in your JetBot
1. Build a TensorRT model `best_model_reg_resnet18_trt.pth` by following instructions in the notebook.

## Live Demo
1. Open `live_demo_resnet18_trt.ipynb`
1. Run your JetBot with the TensorRT model `best_model_reg_resnet18_trt.pth` by following the instructions in the notebook.
