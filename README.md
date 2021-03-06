# antisleep

This is a code for the Antisleep projects that was done as part of my studies at the joint 1 year program in Computer Science and Data Science. The program was organized by the Yandex School of Data Analysis, JetBrains and Computer Science Center. 

The idea of the current project is to perform analysis of dangerous behaviour of people while driving. There are multiple ways to do it, but here I just undertake one possible way which consists of following steps:

- Detect face on a frame (image/video)
- Crop the face
- Detect the landmarks
- Calculate the head's position angles (pitch, yaw, roll) and define whether it corresponds to "dangerous", "unexpected" angle or not.

# References
The code is basically a pipeline that was "constructed" out of other repositories. 
Clearly, they all shall be cited. 

The driving horse is the paper: "PFLD: A Practical Facial Landmark Detector" and here is the link to it: https://arxiv.org/abs/1902.10859

I used the code from its implementation in PyTorch: https://github.com/polarisZhao/PFLD-pytorch. It contains a trained model, and a code to perfrom inference.

Additionally, I used the `kaggle` code for running a MTCNN model for face detection. The code is taken from here:
https://www.kaggle.com/timesler/fast-mtcnn-detector-55-fps-at-full-resolution

I adapted the code from both sources to create the pipeline, although the changes are not drastic.



