# breast-cancer-classification

# **File and Folder Descriptions**
**make_data:** In this section, we prepared the initial dataset. We started with approximately 150 biopsy images, which we divided into smaller fragments of size 50x50 pixels. Each fragment was then labeled as either "0" (no cancer cells) or "1" (presence of cancer cells). The images were organized into separate "0" and "1" folders.

**perform_images:** Here, we selected a sample of 5000 images for analyzing color distributions. We examined the overall, blue, green, and red color content to identify any noticeable differences between the images.

**final_model:** This section contains the file where we trained the final model. The model consists of 2 levels and is based on the DenseNet121 architecture, a neural network model. The training and implementation were done using the Keras package. The model achieved an accuracy of 0.88 based on the AUC (Area Under the Curve) metric.

# **Steps to Reproduce Results**
To reproduce the results of our project, follow these steps:

Data Preparation: Gather biopsy images labeled with "0" and "1" folders. Preprocess the images by dividing each into 50x50 pixel fragments.

Data Combination: Merge all the images into a single folder, while keeping the "0" and "1" folder structure intact.

Data Split: Divide the combined dataset into training, testing, and validation sets, maintaining the original ratio of 1:3.

Color Distribution Analysis (optional): If desired, use the "perform_images" section to analyze the color distributions in the sample of 5000 images.

Model Training: Utilize the file in the "final_model" section to train the neural network model using the Keras package on your prepared dataset.

# **Links to the data and the models:**
data source:
https://www.kaggle.com/datasets/paultimothymooney/breast-histopathology-images

model before fine tuning:
https://drive.google.com/file/d/1VAuG4wQcFEe0qoMJooerGYjyd3sq-3i1/view?usp=sharing

model after fine tuning:
https://drive.google.com/file/d/1UgeYwg2QNBHnNBxQVOAPdDOBVI0ONMxp/view?usp=sharing
