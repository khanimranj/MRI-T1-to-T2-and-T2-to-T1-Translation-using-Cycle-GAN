# MRI-T1-to-T2-and-T2-to-T1-Translation-using-Cycle-GAN
 Generative adversarial model(modified U-Net) which can generate artificial MRI images of different contrast levels from existing MRI scans.
Project Overview
Misdiagnosis in the medical field is a very serious issue but it’s also uncomfortably common to occur. Imaging procedures in the medical field requires an expert radiologist’s opinion since interpreting them is not a simple binary process (Normal or Abnormal). Even so, one radiologist may see something that another does not. This can lead to conflicting reports and make it difficult to effectively recommend treatment options to the patient.
One of the complicated tasks in medical imaging is to diagnose MRI(Magnetic Resonance Imaging). Sometimes to interpret the scan, the radiologist needs different variations of the imaging which can drastically enhance the accuracy of diagnosis by providing practitioners with a more comprehensive understanding.
But to have access to different imaging is difficult and expensive. With the help of deep learning, we can use style transfer to generate artificial MRI images of different contrast levels from existing MRI scans. This will help to provide a better diagnosis with the help of an additional image.
In this project, we will use CycleGAN to translate the style of one MRI image to another, which will help in a better understanding of the scanned image. Using GANs we will create T2 weighted images from T1 weighted MRI image and vice-versa.
 
Problem statement: To build a Generative adversarial model(modified U-Net) which can generate artificial MRI images of different contrast levels from existing MRI scans.
NOTE: The T1 and T2 MRI Images included in the dataset are not related in any way since we have an unpaired dataset here.
 
Project pipeline
The project pipeline can be briefly summarized in the following four steps:
•	Data Understanding: Here, we load the data and create the dataset for it.
•	Image Processing: In this step, we process the images using different steps.
•	Model-Building and Training: This is the final step at which we create your Generators and Discriminators using a modified U-Net architecture(similar to CycleGAN). We also have to define the loss function and training step for model training.
