README

This project implements and analyzes Grad-CAM's sensitivity to various backdoor attacks on deep learning models. The implementation uses PyTorch, and the ResNet50 model fine-tuned on the Oxford-IIIT Pet Dataset serves as the base model. Different backdoor triggers, including a triangular dot pattern, are injected into the dataset to evaluate Grad-CAM's ability to detect and highlight regions responsible for misclassification.

Contents of the Project:
1. **Clean_Model**: Contains the trained clean ResNet50 model.
   - `Clean_Model/clean_model_resnet50.pth`: The model weights for the clean ResNet50 model.

2. **Backdoor_attack1**: Implements a basic backdoor attack with red stripe trigger.
   - `Backdoor_attack1/basic_attack.ipynb`: Jupyter notebook for the backdoor attack.
   - `resnet50_backdoored.pth`: Model weights for the backdoored model.

3. **Backdoor_attack_triangle**: Implements a triangle-based backdoor attack.
   - `Backdoor_attack_triangle/Triangle_attack.ipynb`: Jupyter notebook for the triangular pattern backdoor attack.
   - `resnet50_backdooredtriangle.pth`: Model weights for the triangular backdoored model.

4. **Additional Files**:
   - This README.txt file.
   - COPYRIGHT.txt: Licensing and copyright information.
   - USAGE.txt: Instructions for running the code and understanding the outputs.

For more information, refer to the documentation in `USAGE.txt`.
