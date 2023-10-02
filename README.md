# LynxAI_app

LynxAI, Inc

Connect us at support@lynxai.io


## Introduction
Common AI workflow has a model generation for training and a model inference for deploying the model. The model generation requires GPU for faster execution.

## LynxAI's Solution
Our solution is targeted towards accelerating hardware development.  The LynxAI_app has the model training and model inference (si_twin) integrated into one App.
The app is build on the foundation that enables the user to have full control on the training data.

[LynxAI_app](https://github.com/lynxai-eng/LynxAI_app/blob/main/LynxAI_App.pdf)
## Installation
- Python3.9 required
- This is a Linux release of LynxAI app. Please contact LynxAI for other OS support at support@lynxai.io

clone repository

```bash
    git clone https://github.com/lynxai-eng/LynxAI_app.git
```

install packages 
```bash
    cd LynxAI_app
    pip install -r requirements.txt
```

# Usage/Examples

Input file Example


-  Execute following command to run the app

```bash
    python3 LynxAI_app.py 
```
## LynxAI_app  interface 
- Select one of the options:
1. Training (requried email verification )
2. Si_twin

![alt text](https://github.com/lynxai-eng/LynxAI_app/blob/main/example/1_1.png)
### If you seclect "Training"   

- You need to provide following information:
1) Folder to create/save the model
2) File containing list of signals (please refer to /example/signal for more details)
3) Location (path) of the VCD file

![alt text](https://github.com/lynxai-eng/LynxAI_app/blob/main/example/1_2.png)
![alt text](https://github.com/lynxai-eng/LynxAI_app/blob/main/example/1_3.png)
### If you seclect "Si_twin" 
- You need to provide following information:
1. "model list" (created in the model folder)
2. The location (path) of the test VCD file
3. File containing list of signals (please refer to /example/signal for more details)

![alt text](https://github.com/lynxai-eng/si_twin/blob/main/1.png)

- The GUI displays the result of the model. 
1. The top left window shows the accuracy of the model output against the anticipated output from the Ethernet MAC API. 
2. The Top right displays the failing signals, on a scale of 0 to 1, with 1 being 100% match. For example a signal that is 0.8 indicates  80% success.
3. The bottom window is drilling down into specificity of the failing cycles and the states for which they are failing

![alt text](https://github.com/lynxai-eng/si_twin/blob/main/2.png)
- The VCD file is generated in the following folder

![alt text](https://github.com/lynxai-eng/si_twin/blob/main/3.png)
- After execution new folder will be created as follows: 
```bash
    infer000{n}    // example infer0001,infer0002....
```



 
![Logo](https://lynxai.io/wp-content/uploads/2021/11/AynxAi-Logo-design-final-min-1536x1536-1.png)


## Feedback

If you have any feedback, please reach out to us at support@lynxai.io