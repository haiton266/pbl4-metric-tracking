# Note: myenv of TrackEval is different with Boxmot

# Running the MOT Challenge Script

This document provides a step-by-step guide on how to set up and run the MOT (Multiple Object Tracking) Challenge script specifically for the MOT15 benchmark using Python 3.7.

## Requirements

- Python 3.7
- Virtualenv

Ensure Python 3.7 is installed on your system and accessible from the command line. The instructions below assume Python 3.7 is installed at `C:\Users\haike\AppData\Local\Programs\Python\Python37\python.exe` on a Windows system. Adjust the path according to your installation.

## Setup Instructions

1. **Create a Virtual Environment**

   Open your command line interface and navigate to the directory where you want to set up the project. Then, create a virtual environment named `myenv` using Python 3.7 with the following command:

```
virtualenv --python="/[link]/python.exe"
```

2. **Activate the Virtual Environment**

Activate the virtual environment by running:

- On Windows:
  ```
  myenv\Scripts\activate
  ```

3. **Install Dependencies**

Ensure all required dependencies for the script are installed. This might include libraries such as `numpy`, `pandas`, or specific packages related to the MOT challenge. The exact installation commands may vary.

```
pip install -r requirements.txt
```

## Running the Script

After setting up the environment and installing all dependencies, you can run the MOT challenge script with specific parameters. Use the following command:

This command runs the script for the MOT15 benchmark, evaluates the `train` split, evaluates the `MPNTrack` tracker, calculates the `HOTA`, `CLEAR`, `Identity`, and `VACE` metrics, and runs without parallel processing.

## Customizing the Script

To choose a different file or modify settings:

- **Editing Sequence Maps**: If you want to choose a different file to run, edit the sequence map located at `data\gt\mot_challenge\seqmaps\MOT15-train.txt`. This allows you to specify which sequences are included in the evaluation.

- **Ground Truth and Tracker Data**: Ensure that the ground truth data and tracker outputs are correctly placed in the `data` directory, following the structure expected by the script (`data\gt\mot_challenge\` for ground truth and a similar structure for tracker data).

For more detailed customization, refer to the script's documentation or source code.

```

```

```

```

```

```
