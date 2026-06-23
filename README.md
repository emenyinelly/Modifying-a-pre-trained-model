# Modifying-a-pre-trained-model


# Transfer Learning with VGG16

This project applies transfer learning using the pre-trained VGG16 model on a new image classification dataset. The base VGG16 layers are used as a feature extractor with `include_top=False`, and a custom classifier head is added for the final prediction task.

## Training Process
- **Phase 1:** Freeze the VGG16 base and train only the new classifier layers.
- **Phase 2:** Unfreeze the top layers of VGG16 and fine-tune the model with a lower learning rate.

## Goal
The goal is to reuse features learned from ImageNet and adapt them to a new dataset with better training efficiency and improved classification performance.

## Model Structure
- VGG16 convolutional base.
- Flatten layer.
- Dense layer.
- Dropout layer.
- Softmax output layer.

## Result
The model is evaluated using accuracy and validation accuracy to check how well it performs on the new task.
