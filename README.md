# Captcha-Detection-Mosaic-Ps1
## Made Under Udyam-Mosaic 2022 organised by the Electronics Engineering Society, IIT BHU

## Summary:
The main goal of this project was to develop a model to recognize the CAPTCHA Characters and print the result with minimum error possible. The character set included the english Alphabets (a-z, A-Z) and certain special characters such as Sun, Cloud, etc to name a few. These special characters were mapped to certain digits (0-9). 

## Model Working and Pipeline Model:
### Step 1: Model Definition 
- We made two Deep Learning models for individual analysis of the different character sets.
- The training model for english alphabets [Letter Training Model](Letters_model_training.ipynb)
- The training model for special characters [Emojis Training Model](emoji_model_training.ipynb)
- The accuracy of the letter training model is around **96%** and that of the Emoji traing model is around **96.6%**.

### Step 2: Creating The Final Pipeline
- The Main challenge at this stage was to segment out the Captcha into different Characters.
- For this purpose, we implemented the technique of Vertical Segmentation using OpenCV.
- After getting the Individual Characters, We passed each of them throught the pipeline code and achieved the Final Result.
- The Final Pipeline Model [Pipeline Code](Final_Pipeline.ipynb)
