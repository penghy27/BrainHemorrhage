# Brain Hemorrhage CT Project

This repository contains notebooks and code for detecting and segmenting brain hemorrhages from CT images. The project originated from the course *Machine Learning and Statistical Learning Theory* at Northeastern University and makes use of data provided by Zeta Surgical.

## Directory Structure

- `BrainCTScan_hemorrhage/` – main project folder containing Jupyter notebooks and documentation
  - `BrainCT_CNN_classification.ipynb`
  - `BrainCT_ML_DownSampling_v2.ipynb`
  - `BrainCT_ML_OverSampling_v2.ipynb`
  - `BrainCT_Unet_FinalRun.ipynb`
  - `BrainCT_Unet_PilotRun.ipynb`
  - `Create_Mask_Images.ipynb`
  - `Merge_4windows_Images.ipynb`
  - `FinalProject_Peng_v2.pdf`
  - `README.md` – details of the workflow

## Required Python Packages

The notebooks rely on the following libraries:

- numpy
- pandas
- opencv-python
- tensorflow
- imgaug
- scikit-learn

Install them with:

```bash
pip install numpy pandas opencv-python tensorflow imgaug scikit-learn
```

## Running the Notebooks

1. Prepare the CT scan dataset and labels in a folder similar to the example below. Update the paths inside the notebooks to match your location.

```
CTScan/
  shuffled_images/
    image001.jpg
    ...
  new_hemorrhage_label.csv
  train_set/
    ID_xxx.jpg
    ID_xxx_mask.jpg
  test_set/
    ...
```

2. Launch Jupyter in the project directory:

```bash
jupyter notebook
```

3. Open any notebook from `BrainCTScan_hemorrhage/` and execute the cells in order to reproduce the experiments.
