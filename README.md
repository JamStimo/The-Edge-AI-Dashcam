# The-Edge-AI-Dashcam

This project was developed in order to showcase my knowledge about Edge AI and computer vision using embedded hardware.

Standard AI models are too bulky for a dash cam use, which is why MobileNetV3 was used due to its small size. The AI model was trained on GTSRB (road sign) dataset using PyTorch.

As I did not want to train the AI based on truly pristine (and therefore not similar to a dashcam's) images, additional PyTorch transforms were implemented: GaussianBlur and ColorJitter. The purpose of this is to simulate issues associated with dash cams, such as windshield dirt, motion blurring, or night time operation. Finally, the model was converted into .onnx file, making it actually deployable on edge hardware.

I would like to say this project is purely demonstrative and showcases that I can develop the pipeline in full from PyTorch training to ONNX conversion.
