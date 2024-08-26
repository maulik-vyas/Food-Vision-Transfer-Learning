# Food-Vision-Transfer-Learning

The Dataset used is Food 101 Dataset from Kaggle where 101 food classes are used each with 1000 images (750 for training and 250 for test): https://www.kaggle.com/datasets/dansbecker/food-101

Here, this dataset contains images for 101 different food classes. For simplicity, I have built a transfer learning model using 10 food classes. I used Data Augmentation to augment data and create more harder scenario for model to identify food in various ways. I selected 2 transfer learning models: EfficinetNetV2B0 and ResNet50 but EfficientNetV2B0 performed better than ResNet50 so used that for all experiments. First, I created a feature extraction model for 5 epochs and then fine-tuned by unfreezing few top layers of EfficientNetV2B0 model by running it additional 5 epochs which yielded 0.9168 accuracy.
