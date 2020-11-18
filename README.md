# Brain State Classification with SVM
Use Support Vector Machines to identify brain state from fMRI images

## How to run: 
In the same directory as the test and retest data, run the iPython notebook "brain_classification.ipynb". You will then get an accuracy for the test images, and an accuracy for the retest images.

### Image Preprocessing and Feature Selection:
- Apply a binary mask on all the images to remove background and retain brain voxels only.
- Remove unnecessary features by introducing a variance threshold to the masked data in order to extract the key brain voxels.

### Classification
- The datasets contain 4 states: resting state, finger, lips, or foot movement.
- Support Vector Machine (SVM) is used with different regularization parameters depending on the dataset.
- Introduce a shuffled k-fold cross validation to address imbalance in the class labels and to evaluate model.

